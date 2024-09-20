![World News Collage 2024](https://github.com/user-attachments/assets/ec9b1002-b2a6-418f-901c-4ab61e092cfd)

> Scraping and compiling public news images into a collage.

#

This comprehensive program combines two key functionalities: creating a seamless collage from a folder of images and scraping news-related images from prominent news websites. The collage creation feature takes images from a folder named "Example" and arranges them on a large canvas (5184 x 3546 pixels) with a black background. The goal is to completely cover the background by strategically placing, resizing, and cropping the images to fit into an optimized grid layout. The program calculates the required rows and columns based on the aspect ratio and number of images, while dynamically adjusting horizontal and vertical overlaps to ensure smooth blending and prevent any gaps. The result is a harmonious, gap-free collage saved as "collage.png."

The second functionality automates the process of scraping and downloading images from well-known news sites such as The New York Times, CNN, Reuters, and BBC. Using the requests library for HTTP requests and BeautifulSoup for HTML parsing, the program efficiently gathers image URLs from various sections and subdomains of these websites. It validates each URL to ensure it points to legitimate image files before downloading, handling common image formats like .jpg, .png, and .gif. To avoid overwhelming target websites, it includes delays between requests and employs error handling to manage issues like broken links or network failures. Downloaded images are stored in a designated folder, providing an organized dataset useful for media analysis, research, or machine learning projects. The program's flexible design allows for easy customization of target websites and subdomains, making it adaptable for a range of use cases.

#
### Collage Module

This program generates a collage by strategically placing images from a folder named "Example" onto a large canvas (5184 x 3546 pixels) with a black background. The primary goal is to completely cover the background using all the images, with controlled overlaps to ensure no gaps are visible. The program calculates an optimal grid layout based on the number of images, ensuring each image is resized and, if necessary, cropped to fit its designated space without distortion. By adjusting the horizontal and vertical overlap ratios, the program dynamically determines the cell sizes and overlap dimensions, ensuring that all images blend seamlessly. This precise placement and sizing prevent any part of the black background from showing through, creating a visually appealing, unified collage.

To achieve this, the program first shuffles the images and calculates the required number of rows and columns for the grid, based on the aspect ratio of the collage and the total number of images. Each image is resized and strategically placed with calculated overlaps in both horizontal and vertical directions, ensuring smooth transitions between them. If an image is too large for its cell, the program crops it appropriately, maintaining the clarity and proportion of each image. The final output is saved as a PNG file named "collage.png," which presents a flawless, gap-free composition with all images harmoniously blended together, effectively covering the entire canvas.

#
### News Image Scraper Module

The provided Python program is designed to automate the process of scraping and downloading images from various prominent news websites and their subdomains. By utilizing the requests library for HTTP requests and BeautifulSoup for HTML parsing, the program efficiently extracts image URLs from websites like The New York Times, CNN, Reuters, BBC, and others. It handles multiple subdomains for each news site, ensuring a comprehensive collection of images from different sections of each publication. The program validates each URL to confirm it points to a legitimate image file before downloading, thereby reducing the chances of erroneous data being stored. Additionally, the program uses a systematic approach to avoid overwhelming the target websites by incorporating a delay between successive requests, adhering to ethical scraping practices.

The script also incorporates robust error handling mechanisms to manage issues such as network errors, broken links, or inaccessible resources. It checks each image URL for validity and downloads only those files with common image extensions (.jpg, .png, .gif, etc.), ensuring that only relevant content is collected. By organizing the downloaded images into a designated folder, it provides a structured way to manage and analyze the collected data. This approach is particularly useful for media analysis, research, or machine learning projects that require a large dataset of news-related images. The flexibility to add or modify the list of websites and subdomains makes the script adaptable for various use cases, enhancing its utility for both novice programmers and experienced developers.

#
### Related Links

[Output Blaster](https://github.com/sourceduty/Output_Blaster)
<br>
[Lyrics Collage](https://github.com/sourceduty/Lyrics_Collage)
<br>
[Image Emulator](https://github.com/sourceduty/Image_Emulator)
<br>
[PDF to Image](https://github.com/sourceduty/PDF_to_Image)
<br>
[Extra ChatGPT Images](https://github.com/sourceduty/Extra_ChatGPT_Images)

***
Copyright (C) 2024, Sourceduty - All Rights Reserved.
