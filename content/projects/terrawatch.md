---
title: "TerraWatch - CNN Image Segmentation and Multimodal LLM"
summary: "Proof of concept system developed during the TUM AI Hackathon 2024 to detect deforestation using computer vision and LLMs."
date: 2024-07-26
tags: ["CNN", "LLM", "Python", "React", "Full Stack"]
params:
    image: "path/to/terrawatch-image.png"
    link: "https://github.com/tobiasleibrock/terra-watch"
---

Source code and developer notes are available on [Github](https://github.com/tobiasleibrock/terra-watch)

---

![TerraWatch](/projects/terrawatch/terra-watch.gif)

## About the Project

Deforestation has become one of the leading causes of environmental problems around the world. With the application of vision models on satellite imagery, detection of deforested areas have become easier, however identifying the environmental effects and the causes are still a challenge.

TerraWatch combines computer vision with multimodal LLM models to detect deforestation from satellite images and predict their causes and possible environmental effects.

TerraWatch is a prototype that was built in 48 hours during the TUM AI Hackathon 2024. 

Demo video available on [YouTube](https://www.youtube.com/watch?v=3_woHe52Zwk)

{{< youtube 3_woHe52Zwk >}}

### Architecture

TerraWatch is based on a multi layer infrastructure built upon a Python Flask backend connected to a React frontend app. Combining multiple APIs with custom agent based logic in between the application is able to utilize multiple models and data sources to generate a logical and accurate response to the user, displaying actionable insights directly in the browser. This functionality is setup into multiple steps:

1. Satellite data from Mapbox combined with Geocoding data provided by Nominatim
2. Segmentation using U-NET
3. Biodiversity insights using Llama3-70B and all collected data
4. Final data generation using GPT-4-Turbo with multimodal input data

![terra-watch-architecture.png](/projects/terrawatch/terra-watch-architecture.png)

---

# Technologies Used
- CNN Image Segmentation (U-NET)
- Python (Flask)
- Geocoding (Nominatim)
- Multimodal LLM (GPT-4-Turbo)
- JavaScript (React)
- Mapbox