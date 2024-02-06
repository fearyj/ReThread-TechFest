# ReThread

## Project Story


## Inspiration
As online shopping surges, the fear of buying the wrong clothing size persists due to inconsistent measurements across stores. According to McKinsey, a concerning 70% of returned clothes are due to the wrong sizes rather than defects or quality. To tackle over-purchasing and promote sustainability, we aim to develop a website allowing users to visualize how clothes will fit before purchasing. 

Additionally, the onslaught of throwaway culture of fast fashion in the 21st century calls for greater action towards sustainable practices. By further implementing this system of AI generation into online stores selling pre-loved clothes, users are provided with an additional layer of certainty and thus can be more inclined to buy second-hand items. 

## What it does
By harnessing the power of advanced AI algorithms, our platform empowers users to effortlessly enhance their online shopping experience. By simply uploading a photo of themselves and selecting a clothing item they desire, our innovative technology merges these two images seamlessly. This unique feature allows potential customers to gain a vivid and accurate preview of how the chosen garment will look on their own body. With this virtual try-on capability, we aim to eliminate the uncertainty surrounding online clothing purchases, reducing the likelihood of buying the wrong size, and ultimately promoting more sustainable shopping practices

## How we built it
Generating Images from User's Photo
There will be a model used to generate an image, that takes the user's photo and the information of selected clothing as input. 
After the initial steps of collecting suitable data of User's Photos and Clothing information, we will start the cleaning and preprocessing of data, which will make sure that the data are in the same format and could all be used efficiently. We will be implementing a conditional Generative Adversarial Network (GAN). GANs operate on a competitive framework where a generator creates images from random noise, and a discriminator evaluates whether the image is real or fake. A conditional GAN allows us to condition our generated images on our user’s photos. By modifying the GAN, we take in random noise, clothing information, and the user’s photos as inputs. By introducing random noise, we avoid generating less diverse and predictable images, and allow the generation of natural-looking images. These inputs will help train the generator and the discriminator, until the point where the generator can create realistic and high-quality images. This model will also be integrated to the UI and take in user feedback, to further enhance and fine-tune the model.

Creating a ChatBot 
This ChatBot is for users to consult and seek recommendation of clothing choices.
We will be creating a ChatBot that recommends clothes by using OpenAI's GPT-3 API. We will be taking user inputs for inquiries about what to wear for various occasions. We incorporate GPT-3 to provide contextually relevant replies after preprocessing user inputs. After that, the chatbot integrates apparel data from a database and extracts information from GPT-3's responses. User interactions are managed to provide opportunities for additional queries and explanations. The ChatBot's performance is improved incrementally through a good amount of user testing. This guarantees precise and customized recommendations for the users to reference. This system will be monitored closely and frequently for optimisation and security concerns.

## Challenges we ran into 
Struggling to locate a fitting Open Source API for our envisioned AI system due to the prevalence of private options, we faced an additional challenge with our groupmates' demanding schedules throughout the Hackathon. Compensating for this, we dedicated late-night hours to complete the project. Furthermore, encountering difficulties in downloading packages, we grappled with intricate dependencies, where varying versions yielded disparate results.

## Accomplishments that we're proud of
Despite our groupmate's hectic schedule, we committed to staying up overnight to complete this project. We take pride in our creation, aspiring to reduce the disposal of clothing driven by fleeting fashion trends. Additionally, we are proud of our concept, envisioning a scenario where individuals are eager to experiment with outfits but face limitations due to the exclusive online platform.

## What we learned
We discovered that generating ideas was a straightforward process, yet realized the importance of considering various factors such as project complexity, the busy schedules of our teammates, and their individual strengths and weaknesses. An invaluable lesson emerged: despite the challenges posed by a demanding project, we could consistently rely on each other for support and collaboration.

## What's next for ReThread 
ReThread is an Web App, versatile to be implemented into the world of e-commerce. From second-hand spaces like carousell to TikTok Shop, ReThread can be integrated into familiar user interfaces to provide hyper realistic photos of users in clothes before they add to cart. 

The next versions of ReThread include creating 3D models of the user wearing more clothing types based on true dimensions of the clothing and the user. Taking this further down, an integrated chatbot serves to assist users in finding their perfect fit. Describe the occasion you will be attending and watch as ReThread guides you to your dream outfit: you will never have to say “I don’t know what to wear!”. Virtually try it on, compare products and make your purchase- all with the integration of ReThread.

Based on research done by CoreSight, 24.4% of online apparel orders in the US are returned, amounting to 38 billion US Dollars. In this aspect, ReThread aims to be a game-changer for online retailers like shopee and carousell. By reducing their rate of apparel return, they make sustainable decisions to reduce the transport emissions and cost whilst simultaneously increasing their profit. The use of AI for both the sellers and users translates into a need to redesign how we retrieve clothing.

##  Built with 
* Built with HTML, JS, CSS
* Intend to Incorporate: Generative Adversarial Network (GAN), AWS Cloud Service, OpenAI's GPT-3 API , React Framework


## References:

Chan, A. (2023, April 4). The True Cost of Apparel Returns: Alarming Return Rates Require Loss-Minimization Solutions. Coresight Research. https://coresight.com/research/the-true-cost-of-apparel-returns-alarming-return-rates-require-loss-minimization-solutions/#:~:text=A%2024.4%25%20Online%20Apparel%20Return%20Rate%20Means%20%2438%20Billion%20Returns,-Based%20on%20a&text=Consumers%20who%20shop%20apparel%20and,products%20will%20look%20or%20fit.
‌
Returning to order: Improving returns management for apparel companies. (2021, May 25). McKinsey & Company; McKinsey & Company. https://www.mckinsey.com/industries/retail/our-insights/returning-to-order-improving-returns-management-for-apparel-companies
‌
