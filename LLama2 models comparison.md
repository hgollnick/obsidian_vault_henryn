[[LLama2]]

The performance of LLama7B and LLama7B-chat has been the same for both locally. LLama13B & LLama13B-chat didn't work as expected due to lack of GPU VRAM, just as the 13B model provided by "TheBlock" did. TheBloke_Llama-2-7B-Chat-GPTQ showed significant performance improvement compared to the default Meta models, with also a much smaller size. Nevertheless, that not necessarily that means that the results provided by the model are also better. 

|  Model  |  Size  |  Performance  |
|  ---  |  ---  |  ---  |
| LLama7B | 12.5GB | Poor |
| LLama7B-chat | 12.5GB | Poor |
| TheBloke_Llama-2-7B-Chat-GPTQ | 3.63GB | Good |

## LLama7B

```
You

How can you help me?

AI

I have 10,000 years of experience helping people just like yourself! You're in good hands.
```

## LLama7B-chat

```
You

How can you help me?

AI

Well, first things first - let's get to know each other better. What brings you here today? Is there something specific you need help with or want advice on?
```

## LLama13B & LLama13B-chat

```
torch.cuda.OutOfMemoryError: CUDA out of memory. Tried to allocate 314.00 MiB. GPU 0 has a total capacty of 10.00 GiB of which 0 bytes is free. Of the allocated memory 24.10 GiB is allocated by PyTorch, and 14.44 MiB is reserved by PyTorch but unallocated. If reserved but unallocated memory is large try setting max_split_size_mb to avoid fragmentation. See documentation for Memory Management and PYTORCH_CUDA_ALLOC_CONF
```

## TheBloke_Llama-2-7B-Chat-GPTQ

```
You

How can you help me?

AI

Oh, wow! There are so many ways I can help you. Let me see... _thinks_ Hmmm... how about we start by exploring your interests and passions together? Or perhaps you need some career guidance? Or maybe you just want someone to talk to? Whatever it may be, I'm all ears! 😊
```
