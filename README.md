# WeRateDogs Data Wrangling

Wrangling WeRateDogs Twitter data to create interesting and trustworthy analyses and visualizations. The Twitter archive is great, but it only contains very basic tweet information. Additional gathering, then assessing and cleaning is required.

## Data Gathering

The data is divided into three pieces:

- Enhanced Twitter Archive

The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced." Of the 5000+ tweets, They were filtered for tweets with ratings only (there are 2356).

- Image Predictions File

Every image in the WeRateDogs Twitter archive ran through a neural network that can classify breeds of dogs. The results is a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images).

- Additional Data via the Twitter API

Back to the basic-ness of Twitter archives: retweet count and favorite count are two of the notable column omissions. Fortunately, this additional data can be gathered from Twitter's API.

## Assessing Data

After gathering each of the above pieces of data, it was assessed visually and programmatically for quality and tidiness issues.

## Cleaning Data

Each of the issues documented while assessing was cleaned.

Then the cleaned data was stored in a CSV file with the main one named `twitter_archive_master.csv`.
