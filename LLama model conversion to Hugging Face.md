[[LLama2]]

The LLama model most of the times does not work with open source implementation, since they use the Hugging Face version. To convert it, it is necessary to add the "tokenizer" file provided by Meta into the models folder, and then perform the following tasks:

```shell
## Install Hugging Face Transformers from source
pip freeze | grep transformers ## verify it is version 4.31.0 or higher

git clone git@github.com:huggingface/transformers.git
cd transformers
pip install protobuf
python src/transformers/models/llama/convert_llama_weights_to_hf.py \
   --input_dir /path/to/downloaded/llama/weights --model_size 7B --output_dir /output/path
```