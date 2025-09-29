<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Resume | Specialist Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        /* BASE STYLES: FULL BLUE BACKGROUND, WHITE TEXT */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #2A52BE; /* Full blue background */
            color: #ffffff; /* Default text color set to white for contrast */
        }
        
        /* Ensure all main layout parts inherit or are transparent */
        header, footer {
            background-color: transparent; 
        }
        
        main {
              padding-top: 0;
              background-color: transparent; 
        }
        
        /* Section Headings (H2) */
        .section-heading {
            /* No border-bottom as <hr> tags are removed, keeping padding/margin for spacing */
            padding-bottom: 0.5rem;
            margin-bottom: 1.5rem;
            color: #ffffff; 
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            line-height: 3.0rem;
            font-weight: 700;
        }

        /* Card/Sub-Section Headings (H3) */
        h3 {
            color: #ffffff;
            font-size: 1.5rem;
            line-height: 2.0rem;
            font-weight: 600;
            margin-bottom: 0.25rem;
        }

        /* Sub-sub headings (H4/custom spans) */
        .sub-sub-heading {
            font-size: 1rem;
            line-height: 1.5rem;
            font-weight: 700;
            color: #FFFF00; /* Bright Yellow accent */
        }

        p, span, li {
            color: #e0e0e0; 
            font-size: 0.875rem; 
            line-height: 1.4;
        }
        a {
            color: #90CAF9;
        }
        a:hover {
            color: #BBDEFB;
        }

        .container {
            max-width: 1400px;
        }
        
        /* ADJUSTED PROFILE PICTURE STYLES */
        .profile-picture {
            border-radius: 50%; /* Make it perfectly circular */
            border: 6px solid #fff;
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.2);
            width: 100%; 
            height: 100%; 
            object-fit: cover; 
            object-position: center 25%; /* Adjusted to crop lower body, focus on upper body/knees */
        }
        /* Adjusted to make the profile picture container taller to allow for more vertical space for cropping */
        .md\:w-1\/3 > .flex.justify-center {
            position: relative;
            width: 144px; /* Matches w-36 */
            height: 192px; /* Increased height for mid-shot crop (e.g., 4:3 aspect within a circle) */
            overflow: hidden; /* Ensure content outside the circle is hidden */
            display: flex; /* Flexbox for centering within the container */
            align-items: center; /* Center vertically */
            justify-content: center; /* Center horizontally */
        }
        @media (min-width: 768px) { /* md breakpoint */
            .md\:w-1\/3 > .flex.justify-center {
                width: 192px; /* Matches md:w-48 */
                height: 256px; /* Increased height for mid-shot crop (e.g., 4:3 aspect within a circle) */
            }
        }


        .card {
            background-color: rgba(255, 255, 255, 0.1); 
            padding: 0.75rem 1rem;
            border-radius: 6px;
            box-shadow: 0 1px 4px rgba(0, 0, 0, 0.04);
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            margin-bottom: 0.8rem;
        }
        .text-accent { color: #FFFF00; font-weight: 600; }
        .isbn-highlight { color: #FFFF00; font-weight: 700; } 

        /* Navigation Links Style for Active State */
        .nav-link {
            color: #ffffff;
            font-size: 1rem; 
            padding-top: 0.5rem !important;
            padding-bottom: 0.5rem !important;
            padding-left: 0.6rem !important;
            padding-right: 0.6rem !important;
            border-radius: 4px;
            transition: background-color 0.2s;
            white-space: nowrap; 
        }
        .nav-link.active {
            background-color: #4285F4;
            font-weight: 600;
        }
        
        /* Interactive Sections */
        .content-section {
            display: none;
            animation: fadeIn 0.5s ease-in-out;
            max-height: calc(100vh - 120px); 
            overflow-y: auto; 
            padding-right: 5px;
            background-color: #2A52BE; 
        }
        .content-section.active {
            display: block;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(3px); }
            to { opacity: 1; transform: translateY(0); }
        }
        /* Style for the scrollbar in content sections for better visibility */
        .content-section::-webkit-scrollbar {
            width: 8px;
        }
        .content-section::-webkit-scrollbar-thumb {
            background-color: rgba(255, 255, 255, 0.3);
            border-radius: 4px;
        }
        .content-section::-webkit-scrollbar-track {
            background-color: rgba(0, 0, 0, 0.1);
        }
        
        /* ADJUSTED GALLERY IMAGE STYLES FOR UNIFORM FRAMES */
        .relative.group {
            position: relative;
            width: 100%;
            padding-bottom: 100%; /* Makes the container a perfect square based on its width */
            height: 0; /* Resets height to make padding-bottom effective */
            overflow: hidden; /* Hides any overflow from the image */
            border: 2px solid #fff; /* Optional: Add a border for definition */
            box-sizing: border-box; /* Include padding and border in the element's total width and height */
        }
        .gallery-image { /* This targets the <img> inside the .relative.group */
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover; /* Ensures the image fills the square, cropping as needed */
            display: block;
        }
        /* Specific adjustment for the nitw.png image to focus on faces */
        .nitw-gallery-image {
            object-position: center; /* Tries to center the content */
            /* If faces are at the top, you might try object-position: center top; */
        }


    </style>
</head>
<body class="flex flex-col min-h-screen">

    <header class="shadow-md py-3 sticky top-0 z-50">
        <div class="container mx-auto px-4 md:px-2">
            </div>
        
        <div class="container mx-auto px-4 md:px-2 flex flex-col md:flex-row justify-center items-center header-nav-container">
            <nav class="flex justify-center md:space-x-1 space-x-2 mt-2 md:mt-0 text-sm overflow-x-auto">
                <a href="#about" class="nav-link active" data-target="about">Home</a>
                <a href="#experience" class="nav-link" data-target="experience">Experience</a>
                <a href="#education" class="nav-link" data-target="education">Education</a>
                <a href="#research" class="nav-link" data-target="research">Research</a>
                <a href="#publications-detail" class="nav-link" data-target="publications-detail">Publications</a>
                <a href="#skills" class="nav-link" data-target="skills">Skills</a>
                <a href="#extracurricular" class="nav-link" data-target="extracurricular">Activities</a>
                <a href="#gallery" class="nav-link" data-target="gallery">Gallery</a>
                <a href="#contact" class="nav-link" data-target="contact">Contact</a>
            </nav>
        </div>
    </header>

    <main class="flex-grow">
        <div class="container mx-auto px-6 py-4"> 
            
            <section id="about" class="content-section active">
                <div class="text-center md:flex md:items-center md:text-left">
                    <div class="md:w-1/3 flex justify-center mb-4 md:mb-0 md:mr-6">
                        <img src="https://cdn.jsdelivr.net/gh/sushmitha-d-nitw/Dr.D.SUSHMITHA/website%20phototes/main.png" alt="Dr. D. Sushmitha Profile Picture" class="profile-picture w-36 h-36 md:w-48 md:h-48">
                    </div>
                    <div class="
