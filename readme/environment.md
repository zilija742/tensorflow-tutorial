1. Install python-3.9.10-amd64.exe
2. Install Tensorflow with pip
    System requirements
        - Python 3.7–3.9
            Python 3.9 support requires TensorFlow 2.5 or later.
            Python 3.8 support requires TensorFlow 2.2 or later.
        - pip 19.0 or later (requires manylinux2010 support)
        - Windows 7 or later (64-bit)
        - Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019 (install VC_redist.x64.exe)
        - GPU support requires a CUDA®-enabled card (Ubuntu and Windows)
    2.1. Install the Python development environment on your system
        Check if your Python environment is already configured:

            Requires Python 3.7–3.9, and pip >= 19.0

            python --version
            pip --version
        
        Install the Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017, and 2019. Starting with the TensorFlow 2.1.0 version, the msvcp140_1.dll file is required from this package (which may not be provided from older redistributable packages). The redistributable comes with Visual Studio 2019 but can be installed separately:

            - Go to the Microsoft Visual C++ downloads,
            - Scroll down the page to the Visual Studio 2015, 2017 and 2019 section.
            - Download and install the Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019 for your platform.
        Make sure long paths are enabled on Windows.
        Install the 64-bit Python 3 release for Windows (select pip as an optional feature).

    2.2 Create a virtual environment (recommended)
    Python virtual environments are used to isolate package installation from the system.

        - Create a new virtual environment by choosing a Python interpreter and making a .\venv directory to hold it:
            
            python -m venv --system-site-packages .\venv

        - Activate the virtual environment:

            .\venv\Scripts\activate

        - And to exit the virtual environment later:

            deactivate  # don't exit until you're done using TensorFlow
    
    2.3 Install the TensorFlow pip package