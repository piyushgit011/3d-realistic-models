# 3d hyper-realistic models
Project 1: Transforming Mannequins into Photorealistic Models
Repo:  https://colab.research.google.com/drive/1VU0sQ99VHOj2j0vXMHkXwr0O-AAc7v6h?usp=sharing
Project Overview:
This initiative aims to transform mannequins into lifelike models through advanced image processing techniques. The primary objective is to reduce the financial burden on sellers associated with traditional model photoshoots by leveraging state-of-the-art AI models for generating realistic images.
Flowchart:

Technical Approach:
Model Selection for Detection and Segmentation:
Grounding DINO: Utilized for generating precise masks for inpainting tasks, facilitating accurate delineation of the mannequin and clothing items. Grounding DINO GitHub
Segment Anything Model: Employed for its robust capability to segment various objects within an image, essential for isolating the mannequin from the background. Segment Anything GitHub
Grounded Segment Anything: Combines the strengths of grounding and segmentation to create detailed masks of the mannequin's body and head. Grounded Segment Anything GitHub
Cloth Segmentation Model (U2Net): Specifically used for the segmentation of clothing, ensuring the fabric's texture and form are accurately captured. Cloth Segmentation GitHub
Mask Creation Process:
The process involves combining the head and body masks while subtracting the cloth segmentation to retain only the mannequin's figure. The head mask is derived from head detection algorithms, converting detection boxes into masks. Similarly, the body mask is obtained through person detection and segmentation techniques. The cloth segmentation is accomplished using the U2Net model, tailored for textile attributes.
Photorealistic Image Synthesis:
Stable Diffusion Models: The project employs Juggernaut XL and Realistic Vision V6.0, both fine-tuned versions of stable diffusion models known for their high-quality, lifelike image generation capabilities.
Juggernaut XL on Hugging Face
Realistic Vision V6.0 on Hugging Face
Fooocus API Integration: Enhances the image generation process by incorporating LoRA and IP adapters, resulting in more refined and accurate visual outputs. The Fooocus API serves as a bridge to the Fooocus image generation software, optimizing the model's performance for this specific application.
Fooocus API GitHub
Fooocus Software GitHub
The combination of these sophisticated models and techniques culminates in the creation of photorealistic images where mannequins are seamlessly transformed into human models, offering a cost-effective and scalable solution for digital fashion showcases.
For a detailed walkthrough of the process and to view sample outputs

![1](https://github.com/piyushgit011/3d-realistic-models/assets/96625965/0d98a887-d517-4231-952c-2f39e399cf73)

![4](https://github.com/piyushgit011/3d-realistic-models/assets/96625965/61b20da3-db1e-429a-85bc-a650b4bb72aa)

![7](https://github.com/piyushgit011/3d-realistic-models/assets/96625965/52865ec9-c283-4d78-b5bc-2826997fdaa8)




