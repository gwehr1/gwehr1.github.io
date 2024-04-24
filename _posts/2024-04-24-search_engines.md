# Search Engines for Dataset Collection
The process of building datasets for deep learning applications is arguably the most important step. As I've been told:
> "If you put rubbish in, you'll get rubbish out..."

This step can also be super labor-intensive and time-consuming if you collect images manually one by one from a web browser, however, as I've recently learnt, leveraging search engines such as DuckDuckGo can significantly speed up this process.

## Method
This approach involves collecting images directly through the search engine using **only a single line of code**.
The key import is: 
```
from duckduckgo_search import DDGS
```

Then the key command (passing in a search term and max number of images) to call is:
```
DDGS(search_term, max_results=max_number_images)
```

## Benefits
Using DuckDuckGo search not only simplifies the gathering of data either, but also increases the efficiency of the subsequent steps involved in dataset preparation!

1. Simplified Data Acquisition:
Using DuckDuckGo to search for images enables the acquisition of large volumes of data without the need to manually search for and download each image individually. This approach can save considerable time and effort, especially when dealing with large datasets.

2. Integration with DataBlocks:
DataBlocks are a programming structure used to define how data is processed and prepared for training in machine learning applications. By obtaining images through a search engine, these can be directly fed into DataBlocks. This allows for automated preprocessing steps such as resizing, normalization, and augmentation, which are essential for preparing the images for model training.

3. Preliminary Sanity Checks:
When images are sourced through a search engine, initial checks regarding the relevance and quality of these images can be performed automatically. This "sanity check" ensures that the images are suitable for the intended application, thus filtering out irrelevant or low-quality data at an early stage.

4. Automated 'Labeling':
Perhaps one of the most significant advantages of using a search engine for dataset collection is the potential for automated labeling. Images sourced through DuckDuckGo often come with associated metadata, which can include labels. These labels can be used as initial data points for supervised learning models, reducing the need for manual labeling, which is often resource-intensive and prone to human error.

> [!IMPORTANT]
> While this method provides a good starting point for dataset collection, it is important to recognize that the automatically generated labels and image quality may not always meet the strict criteria required for specific analytical tasks. Therefore, it is advisable to supplement this approach with manual review and refinement to ensure the dataset’s quality and applicability to the task at hand.
