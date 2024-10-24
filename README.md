# Not Just Question-Answering! A Framework for Video-LLM Capability Augmentation

## Structure


## Usage

In the file `main.ipynb`, you can see the following code snippet:

```python
from vlm_cv import Agent

agent = Agent(gemini_api_key='your_gemini_api_key', hf_api_key='your_hf_api_key', verbose='normal')

# optional configuration
agent.max_tokens = 300
agent.temperature = 0
agent.model_timeout = 20000

response, image = agent.call_agent(video='./inputs/video_dog.mp4', query="What's close to the dog?")

print("Response:", response)
image.show()
```
