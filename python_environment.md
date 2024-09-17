# How to setup a local notebook kernel to enable GPU training

This is from chatGPT and it works well.

### Step 1: Create a Python Virtual Environment
Open a terminal (PowerShell/Command Prompt) in the directory where you want to create your virtual environment.

Run the following command to create a virtual environment named myenv (you can replace myenv with any name):
``
python -m venv myenv
``

Activate the virtual environment:
On Windows, run:
`myenv\Scripts\activate`
- If you need permission to run script on windows PS, use this command: `Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
`

On Linux/macOS, run:
`source myenv/bin/activate`


Once activated, you should see (myenv) at the beginning of your terminal prompt, indicating that the virtual environment is active.

### Step 2: Upgrade pip and Install Required Libraries
Upgrade pip to the latest version to ensure smooth installation of other packages:

`python -m pip install --upgrade pip`

Install PyTorch with CUDA support. Since you have CUDA 12.6, we'll install the appropriate version of PyTorch compatible with your CUDA version.

As of now, PyTorch does not yet officially support CUDA 12.6, but support for the latest CUDA versions is frequently updated. To install a version compatible with the latest CUDA version supported by PyTorch (typically CUDA 11.x), you can run:

`pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118`
This installs PyTorch with CUDA 11.8 support, which should work on your setup if the drivers are backward-compatible.

### Step 3: Verify Installation
After installation, you can check if PyTorch recognizes the CUDA-enabled GPU by running the following Python code:

```
import torch

print(f"CUDA is available: {torch.cuda.is_available()}")
if torch.cuda.is_available():
    print(f"CUDA Version: {torch.version.cuda}")
    print(f"Device: {torch.cuda.get_device_name(0)}")
This will confirm if PyTorch is properly set up and whether CUDA is available for computation on your GPU.
```

### Step 4: Fix Potential Issues
If PyTorch doesn't detect the GPU or CUDA is unavailable, it may be due to:

- PyTorch and CUDA version mismatch: You can always check PyTorch’s installation page for up-to-date compatibility details.
- Driver issues: Run nvidia-smi in PowerShell to check if your GPU and drivers are functioning correctly.
- Updating NVIDIA drivers: Ensure that your NVIDIA drivers are updated to the latest version. You can download the latest drivers from the NVIDIA driver download page.
  
### Step 5: Deactivating the Virtual Environment
Once you're done working in the virtual environment, you can deactivate it with the following command:

`deactivate`