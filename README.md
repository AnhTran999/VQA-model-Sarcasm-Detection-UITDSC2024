# VINTERN 1B

## Cấu trúc các file
- `a_up_sample.ipynb`: 
    - up samples dựa trên data gốc
    - dựa trên công thức sau: text-only = multi.text + no.image, image.only = multi.image  + no.text
- `b-finetuning.ipynb`:
    - phần này chủ yếu: là tìm cách đưa data về format conversation của model gốc, sau đó chỉ việc chỉnh path và finetuning
    - setup môi trường có thể hơi tricky vì phần requirements của OpenGVLab không ghi rõ version, mình có thể phải down version của 2 thằng accelerate hoặc transformers. Code chỉ chạy được ở trên GPU.
- `c-inference.ipynb`: load lại model đã finetuning và submit

## Ref
- [Vintern-1b](https://huggingface.co/5CD-AI/Vintern-1B-v2#vintern-1b-v2-%E2%9D%84%EF%B8%8F-viet-internvl2-1b-v2---the-llava-%F0%9F%8C%8B-challenger)
