# Landing Page for [Your Discord Name]

This is a modern, feature-rich landing page for a Discord server, designed to be hosted for free on GitHub Pages.

![Page Preview](URL_OF_YOUR_SCREENSHOT)
*(Tip: Once the site is live, take a screenshot and replace the URL above for a nice preview)*

## 🎨 Features

- **Modern & Dark Design**: A stylish interface that highlights your community.
- **Fully Responsive**: Adapts perfectly to desktops, tablets, and mobile devices.
- **Dynamic Animations**: Fade-in effects on scroll and animated statistics to showcase server activity.
- **Rich Content Sections**: Includes sections for server purpose, rules, community showcase, and staff members.
- **Self-Contained**: A single `index.html` file, easy to modify and deploy.

## 🔧 How to Customize

This guide explains how to edit each part of the page.

### Basic Configuration

1.  **Server Name**: Open `index.html` and find and replace all occurrences of `Your Discord Name` with your server's actual name.
2.  **Invite Link**: Find the line containing `href="https://discord.gg/YOUR_LINK"` and replace `YOUR_LINK` with your permanent invite code.
3.  **Introductory Texts**: Edit the paragraphs in the "Who We Are" and "Our Server's Mission" sections to fit your community's purpose.

### Statistics Section

The numbers in this section are animated automatically. To change the final values:
- Find the `data-goal="..."` attribute for each of the three stats.
- Change the number inside the quotes to your desired value.

**Example:** To set the member count to 2,500, change this:
```html
<p class="text-5xl font-bold text-blue-400" data-goal="1250">0</p>
```
To this:
```html
<p class="text-5xl font-bold text-blue-400" data-goal="2500">0</p>
```

### Community Showcase Section

This section contains placeholders for your screenshots.
- Replace the placeholder `<div>` blocks with your own `<img>` tags.
- For best results, use images with a 16:9 aspect ratio.

**Example:**
```html
<div class="showcase-image rounded-lg"><span>Your Screenshot Here</span></div>

<img src="your-screenshot-1.jpg" alt="A screenshot from our server" class="rounded-lg object-cover">
```

### Rules & Team Sections

- **Rules**: Simply edit the titles and descriptions inside the three rule cards to match your server's guidelines.

- **Team**: For each staff member, replace the placeholder avatar `<div>` with an `<img>` tag and edit the name and role.

**Example:**
```html
<div class="text-center">
    <div class="w-32 h-32 bg-gray-700 rounded-full mx-auto mb-4 flex items-center justify-center">
        <span class="text-gray-500 text-sm">Avatar</span>
    </div>
    <h3 class="text-xl font-bold text-white">Alex</h3>
    <p class="text-purple-400">Server Owner</p>
</div>

<div class="text-center">
    <img src="avatar-of-alex.png" alt="Avatar of Alex" class="w-32 h-32 rounded-full mx-auto mb-4 object-cover">
    <h3 class="text-xl font-bold text-white">Alex's Real Name</h3>
    <p class="text-purple-400">Server Owner</p>
</div>
```

## 🚀 Deployment on GitHub Pages

Host your site for free in minutes:

1.  Create a new repository on [GitHub](https://github.com/new).
2.  Click on `uploading an existing file` and drop your `index.html` and `README.md` files (and any images you added).
3.  Once the files are uploaded, go to the **Settings** tab of your repository.
4.  In the left menu, click on **Pages**.
5.  Under "Branch", select the `main` branch and leave the folder as `/root`. Click **Save**.
6.  Wait a few minutes. Your site will be available at the address: `https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/`
