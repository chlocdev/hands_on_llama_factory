# setup

- create conda virtual environment: `conda create -n <your_virtual_environment_name>`

- installation [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory): 

        git clone https://github.com/hiyouga/LLaMA-Factory.git
        cd LLaMA-Factory
        pip install -e ".[torch,metrics]"

*Extra dependencies available: torch, torch-npu, metrics, deepspeed, bitsandbytes, hqq, eetq, gptq, awq, aqlm, vllm, galore, badam, qwen, modelscope, quality*

**Tip** *Use `pip install --no-deps -e .` to resolve package conflicts.*

- test the installation `llamafactory-cli help`
