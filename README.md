R
### Installation

1.  **Clone the Repository**:

    `git clone https://github.com/Rohitdamerr/my-portfolio.git cd portfolio`

2.  **Install Dependencies**:

    `npm install # or yarn install`

3.  **Customize data.json**:
    -   Open data/data.json and update the fields with your information:

`
{ "data": { "navtext": "Your Name", "email": "your.email@example.com", "projects": [ { "projectType": "Project Type", "title": "Project Title", "description": "Project description.", "techStack": ["tech1", "tech2"], "image": "/images/project-image.png", "liveLink": "https://project-live-link.com", "githubLink": "https://github.com/your-username/project", "category": "Category (e.g., Full Stack, React)" } ] } }
`

    -   Add your projects, skills, and other details as needed.
4.  **Add Assets**:
    -   Place your profile picture, project images, and tech stack icons in the public/images/ and public/icons/ directories.
    -   Replace public/background/bgvideo.mp4 with your hero section video (or keep the existing one).
    -   Compress the video using FFmpeg for better performance:


        `ffmpeg -i your-video.mp4 -c:v libx264 -preset veryslow -crf 18 -vf scale=1280:720 -an -pix_fmt yuv420p public/background/bgvideo.mp4`

    -   Add a fallback image (public/poster-bgvideo3.jpg) for the video.
5.  **Run the Development Server**:

    `npm run dev # or yarn dev`

    Open <http://localhost:3000> to view the site.
6.  **Build and Deploy**:
    -   Build the project:

        `npm run build # or yarn build`

    -   Deploy to Vercel or your preferred hosting platform:

        `vercel deploy`

📬 Contact
----------

-   **Name**: Rohit Damer
-   **Email**: <rohitdamer2006@gmail.com>
-   **GitHub**: [github.com/Rohitdamerr](https://github.com/Rohitdamerr)
-   **Portfolio**: [rohitdamer.vercel.app](https://rohitdamer.vercel.app)