# ABaC analysis reviews

The goal of this project is to perform a Sentiment Analysis from reviews to the Catalan restaurant [ABaC Restaurant](https://abacbarcelona.com/es/restaurante) from Jordi Cruz (a Spanish famous chef). The reviews are extracted from [TripAdvisor](https://www.tripadvisor.com/Restaurant_Review-g187497-d1074448-Reviews-ABaC-Barcelona_Catalonia.html) through [Web scraping](/webscraping.ipynb)

As most of the reviews are in Spanish and the pretrained models that will be used are set up in English, next step is to translate the reviews to English. To do so, Systran Translate helps us to perform that task, also using Web Scraping (as they do not have a free API). [Translation function](/translation.ipynb)

Once every review is in English, to perform a Sentiment Analysis we will use transformers from [Hugging Face](https://huggingface.co/). Transformers provides thousands of pretrained models to perform tasks on texts such as classification, information extraction, question answering, summarization, translation, text generation and more in over 100 languages. Its aim is to make cutting-edge NLP easier to use for everyone.

And after each review is classified into positive, negative and neutral, a simple Word Cloud will be performed to see what are customers most of the time talking about.

Which benefits can a Sentiment Analysis offer to a restaurant or to another business?

- **Improve Customer Service.** What does your customers really desire? What are their main complaints? And possiby reply to the bad reviews to find out more.

- **Develop Quality Products.** What do your customers wish your product had? Find out what is the main bottleneck of your product.

- **Improve Media Perceptions.** What's the overall feeling about your product? How do customers behave with your product and the one from your competitors?