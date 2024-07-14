# Overview

This README provides information about the Trends API hosted at [https://trendserver.onrender.com/trends](https://trendserver.onrender.com/trends). This API is used to fetch the latest trends currently ongoing and easily bypasses CORS issues. It is hosted on Render for reliable access and easy implementation.

# Features

- **Fetch Latest Trends**: Retrieve the latest trends happening now.
- **Bypass CORS Issues**: Easily bypass CORS restrictions for smoother integration.
- **Hosted and Accessible**: The API is hosted on Render, ensuring reliability and availability.

# Endpoint

### GET /trends

Fetch the latest trends.

**URL**: [https://trendserver.onrender.com/trends](https://trendserver.onrender.com/trends)

**Method**: `GET`

**Response**: A JSON object containing the latest trends. Each trend object includes the following fields:
- `newsUrl`: The URL to the news article.
- `source`: The source of the news article.
- `imageUrl`: The URL of the image associated with the news article.
- `snippet`: A brief snippet of the news article.
- `shareUrl`: The URL to share the trend.
- `endDateForNextRequest`: The end date for the next request.
- `rssFeedPageUrl`: The URL of the RSS feed page.

**Example Response**:
```json
{
  "newsUrl": "https://timesofindia.indiatimes.com/city/kolkata/assembly-bypoll-results-list-of-winning-candidates-in-13-seats-across-7-states/articleshow/111711377.cms",
  "source": "Times of India",
  "imageUrl": "https://t3.gstatic.com/images?q=tbn:ANd9GcTo7Qw0k-uJYY_Ue5tmLkHnaiJtQkfAYf39Ctav7pY-dnFKXKGJA8FkdX6GtfHOTqiSKaOA2Pe3qw",
  "snippet": "The INDIA alliance secured 10 of 13 seats in the by-elections held across seven states. TMC's Krishna Kalyani won Raiganj, while Congress' Kamlesh Tha.",
  "shareUrl": "https://trends.google.com/trends/trendingsearches/daily?geo=IN&tt=Bypoll+Results#Bypoll%20Results",
  "endDateForNextRequest": "20240712",
  "rssFeedPageUrl": "https://trends.google.com/trends/trendingsearches/daily/rss?geo=IN"
}
