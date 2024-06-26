# Investigation-of-Approximate-circuits-in-Deep-Neural-Network
This study explores using approximate arithmetic circuits to enhance DNN energy efficiency via layer-specific multiplier approximations in the AdaPT framework. It reduces power consumption while maintaining high accuracy across various DNN models, advancing energy-efficient AI for diverse environments

**AdaPT** is a fast emulation framework that extends PyTorch to support approximate inference as well as approximation-aware retraining. AdaPT can be seamlessly deployed and is compatible with the most DNNs. You can evaluate the framework on several DNN models and application fields including CNNs, LSTMs, and GANs for a number of approximate multipliers. 

## Dependencies 

* A linux system with docker installed
      
## Quick start 

The project has everything installed inside the provided docker image and the python path is set to the adapt folder to load the modules. 

Run the following commands to get started:

* Run docker container
```bash
./docker/run_docker.sh
``` 

* Run jupyter on port 8888
```bash
./examples/run_jupyter.sh
``` 
Then copy the jupyter link into a browser and head over the examples folder to run the notebooks

Optional:
* The link to download several model weights to test them in the example notebooks is already provided. <br />
 You must save them inside ```examples/models/state_dicts/``` folder. [[link]](https://drive.google.com/drive/folders/1HtxlPWGXG6svdHAs197uIirt0yHLo_tC?usp=sharing)


## References
This project is a modified version of the adapt framework by dimdano. We acknowledge their work as the groundwork for this project. While the core functionality remains similar, we've introduced important modifications by allowing different multipliers per layer, enabling more fine-tuned optimization. If you'd like to explore the original implementation details, you can refer to the project here https://github.com/dimdano/adapt and In addition to the adapt framework, we also reference the following [[paper link]](https://ieeexplore.ieee.org/document/9913212) which provide a deeper understanding of the core concepts behind the framework.

