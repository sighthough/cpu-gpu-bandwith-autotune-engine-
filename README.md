# cpu-gpu-bandwith-autotune-engine-
this is a benchmark that measures your pc's cpu and gpu bandwiths over different chunks and provides a json file you can use in your project to set the optimal sizes for each

*Co-authored by [sighthough](https://youtu.be/UtPiUGwu-0Q) and Gemini 3.6*

How This Works Universally Across SystemsDynamic Metric Evaluation:
When any computer runs this HTML benchmark, the script iterates through buffer sizes and calculates the ratio:$$\text{Cost Ratio} = \frac{\text{Measured Latency (ms)}}{\text{Measured Bandwidth (GB/s)}}$$
It identifies the exact minimum ratio for Low-Latency applications and the true inflection point for Bulk Throughput
on that specific GPU and CPU architecture.JSON Hardware 
Profile Export:
Upon completion, clicking Export System Config (JSON) downloads gpu_memory_config.json. 
Any game engine, web app, or native C++/Rust software can read this file on boot to configure its allocation chunk sizes dynamically.
