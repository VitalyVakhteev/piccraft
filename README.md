# PicCraft

This project aimed to bridge the virtual and real worlds by integrating AI generative technology and NFTs to enhance game experiences, in our case, Minecraft. Most of our process focused on implementing this idea in Minecraft only, as Minecraft provides an excellent base for new Java code.

## Application Flow

The flow of the application functions as follows:

- A Telegram Bot is contacted by a user, with the user beginning a Minecraft artwork process. 
- Users submit an artwork name and description of their choosing, which manipulates the AI's prompt.
- Users also submit a base image (a picture of an object in the real world or just an image) to serve as a base for future image generation.
- Users are also required to enter their server_id, an ID given after they go through a different process to add their Minecraft server running the generative plugin to the project.
- Finally, users enter the coordinates in the game world in the "X,Y,Z" format.

Once all of these variables are complete, the next intended flow is for the image to be submitted to Dall-E for manipulation. The resulting image would then be minted as an ERC721 token on the Canto network, and the NFT's image representation would then be sent in a request to the plugin. After receiving the request, the plugin generates the image in the game world, completing the process.

## Impact

Through this flow, a tangible and unique connection would be formed between real-world objects and virtual worlds. AI generative and NFT technologies can enhance game experiences within games like Minecraft, and this project aimed to demonstrate the tangibility of this idea and its potential.

## Achievements & Plans

Currently, the Telegram bot (@PicCraftBot) has a functioning flow with the ability to submit variables as described above. After submitting variables, it was intended for AI generation and minting to occur.

Unfortunately, due to complications with the underlying Camunda processes used, generative technology was not implemented in time. The Solidity contract present in this repository, to be used for minting, was also unable to be properly integrated. As a result, images are currently rendered in their original form.

Images were also originally intended to be converted into 3D meshes to enable complete structure rendering in Minecraft, but the difficulty of implementing 2D generation alone meant that 3D rendering was shelved for future implementation.

In the future, AI generation and NFT rendering will be completely fleshed out and added. 3D rendering can also be implemented as a second priority, given enough time.

For a quick technical paper, check out [our link](https://drive.google.com/file/d/1p2ermEQWstCXOIDgcE0RF-rVJzBOlOcb/view?usp=sharing).
