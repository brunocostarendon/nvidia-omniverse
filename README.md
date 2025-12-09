## Generating quality driving data with Cosmos 

Generating quality driving data with Cosmos
We provide a short demo using Cosmos-Predict to generate a short driving clip, and Cosmos-Reason to determine if the video is realistic enough for training.

The video is indeed scored as real (=0). If we decide Cosmos-Reason is a good enough critic, we can increase this video's generation to create large datasets for training and set up evaluation benchmarkings, noting their source origin.

We can also argue this video is not of good enough quality. In reviewing the video, we see artifacts propagated from present to future frames, and a large amount of shakiness to the video. We could address the shakiness of the video by using different prompts, fine-tuning a Cosmos-Predict for a single + fixed camera position, or review the datasets used to train this network.
