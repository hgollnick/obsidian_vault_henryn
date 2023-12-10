have manage to run LLama2 through [Text generation Web UI](https://github.com/oobabooga/text-generation-webui) downloading the models from [TheBloke's  Hugging Face repository](https://huggingface.co/TheBloke`). Currently more tests are definitely necessary.  With the model "TheBloke_Llama-2-13B-Chat-fp16" with 16 Million parameters, there is some GPU memory limitations, resulting in the following error:

I successfully ran LLama2 using the [Text Generation Web UI](https://github.com/oobabooga/text-generation-webui) by downloading the models from [TheBloke's Hugging Face repository](https://huggingface.co/TheBloke%60). However, I encountered challenges when using the "TheBloke_Llama-2-13B-Chat-fp16" model with 16 million parameters due to GPU memory limitations. The following error occurred:

`RuntimeError: CUDA error: out of memory CUDA kernel errors might be asynchronously reported at some other API call, so the stacktrace below might be incorrect. For debugging consider passing CUDA_LAUNCH_BLOCKING=1. Compile with TORCH_USE_CUDA_DSA to enable device-side assertions.`

Attempts to address the issue by limiting GPU memory (`--gpu-memory GPU_MEMORY`) and using options like `--auto-devices`, `--disk`, and `--no-cache` were unsuccessful. It seems the model requires more memory than available. Tests with this model don't appear to be worth it with the current know-how of the subject.

 - [x] Try to download and the model provided directly from Meta.

