# llama.cpp/example/tts/csm

## Mimi Tokenizer

To download the weight, do:
```python
from huggingface_hub import snapshot_download
snapshot_download(repo_id="kyutai/mimi", local_dir="./models/mimi")
```

Firstly, convert the huggingface format to gguf:
```console
(venv) python convert_hf_to_gguf.py models/mimi \
    --outfile models/mimitokenizer-f16.gguf --outtype f16
```