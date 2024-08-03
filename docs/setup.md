# setup

- create conda virtual environment: `conda create -n <your_virtual_environment_name> python=3.8`

- installation [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory): 

        git clone https://github.com/hiyouga/LLaMA-Factory.git
        cd LLaMA-Factory
        pip install -e ".[torch,metrics]"

*Extra dependencies available: torch, torch-npu, metrics, deepspeed, bitsandbytes, hqq, eetq, gptq, awq, aqlm, vllm, galore, badam, qwen, modelscope, quality*

**Tip** *Use `pip install --no-deps -e .` to resolve package conflicts.*

- test the installation `llamafactory-cli help`

**Tip** *Remove packages in root environment*

        for package in $(conda list --name base | awk '{print $1}' | tail -n +4)
        do
        conda remove -n base --yes $package
        done

- Initialize Conda (if necessary): `conda init bash`

- Activate conda `conda activate`

- Clean up unused packages and cache: `conda clean --all`