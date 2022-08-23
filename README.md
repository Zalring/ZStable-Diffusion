# ZStable-Diffusion

Colab Stable Diffusion text-to-image and image-to-image synthesis

--

From the Stable Diffusion repo (https://github.com/CompVis/stable-diffusion) :

- Stable Diffusion is a latent text-to-image diffusion model. Thanks to a generous compute donation from Stability AI and support from LAION, we were able to train a Latent Diffusion Model on 512x512 images from a subset of the LAION-5B database. Similar to Google's Imagen, this model uses a frozen CLIP ViT-L/14 text encoder to condition the model on text prompts. With its 860M UNet and 123M text encoder, the model is relatively lightweight and runs on a GPU with at least 10GB VRAM. See this section below and the model card.
- Stable Diffusion v1 refers to a specific configuration of the model architecture that uses a downsampling-factor 8 autoencoder with an 860M UNet and CLIP ViT-L/14 text encoder for the diffusion model. The model was pretrained on 256x256 images and then finetuned on 512x512 images.
- By using a diffusion-denoising mechanism as first proposed by SDEdit, the model can be used for different tasks such as text-guided image-to-image translation and upscaling. Similar to the txt2img sampling script, we provide a script to perform image modification with Stable Diffusion.

--

Special features of this Colab :
- Settings saving
- Better image save management
- Multi-prompts (1 per iteration)
- Make easier to use your txt2img/img2img outputs as img2img inputs (multiple inputs for img2img possible)
- Real-ESRGAN (https://github.com/xinntao/Real-ESRGAN) upscaling and face enhancement
- No NSFW filter.
