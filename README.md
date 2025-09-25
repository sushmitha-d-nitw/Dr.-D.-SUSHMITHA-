<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Resume | Specialist Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        /* FINAL FIXED BACKGROUND COLOR (Blue as primary background: #0066FF) */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0066FF; /* Primary Blue background */
            color: #333;
        }
        /* Content area set to an off-white/very light blue for high readability */
        main {
            background-color: #F0F8FF; 
        }
        h1, h2 {
            font-family: 'Playfair Display', serif;
        }
        .container {
            max-width: 1200px;
        }
        .profile-picture {
            border-radius: 50%;
            border: 6px solid #fff;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
        }
        /* Highly compressed card with increased font sizes */
        .card {
            background-color: #ffffff;
            padding: 0.2rem 0.5rem; /* Reduced padding for extreme compression */
            border-radius: 4px;
            box-shadow: 0 1px 4px rgba(0, 0, 0, 0.04);
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            margin-bottom: 0.3rem; /* Further reduced space between cards */
        }
        .card:hover {
            transform: translateY(-1px);
            box-shadow: 0 3px 8px rgba(0, 0, 0, 0.06);
        }
        .btn {
            padding: 0.6rem 1.6rem; 
            border-radius: 9999px;
            font-weight: 700;
            transition: transform 0.2s ease;
        }
        .btn-projects { background-color: #FF5A5F; color: #fff; }
        .btn-contact { background-color: #4CAF50; color: #fff; }
        .text-accent { color: #0059B3; } 
        .section-heading {
            border-bottom: 1px solid #e2e8f0;
            padding-bottom: 0.4rem;
            margin-bottom: 0.6rem;
            color: #1a202c;
            font-size: 1.5rem; /* Increased H2 size */
        }
        .nav-link.active {
            color: #0059B3;
            font-weight: 700;
            border-bottom: 2px solid #0059B3;
        }
        .content-section {
            display: none;
            animation: fadeIn 0.5s ease-in-out;
            max-height: calc(100vh - 120px); 
            overflow-y: auto; 
            padding-right: 5px; 
        }
        .content-section.active {
            display: block;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(3px); }
            to { opacity: 1; transform: translateY(0); }
        }
        /* Custom styles for extreme horizontal and minimal vertical space */
        .card-content {
            display: flex;
            flex-direction: column;
            line-height: 1.3; 
        }
        .card-content > * {
            margin-top: 0;
            margin-bottom: 0;
            padding-top: 0;
            padding-bottom: 0;
        }
        .horizontal-list {
            display: inline;
            list-style: none;
            padding-left: 0;
            margin-left: 0;
        }
        .horizontal-list li {
            display: inline;
            margin-right: 10px; 
            position: relative;
            padding-right: 10px;
        }
        .horizontal-list li:not(:last-child):after {
            content: "|";
            position: absolute;
            right: 0;
            color: #ccc;
        }
        .gallery-image {
            width: 100%;
            height: 180px; 
            object-fit: cover;
            border-radius: 4px;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <header class="bg-white shadow-sm py-3 sticky top-0 z-50">
        <div class="container mx-auto px-6 flex flex-col md:flex-row justify-end items-center">
            <h1 class="text-xl md:text-2xl font-bold"></h1> 
            <nav class="flex flex-wrap justify-center md:flex-row md:space-x-5 space-x-3 mt-2 md:mt-0 text-sm">
                <a href="#about" class="nav-link py-1 px-3 text-gray-700 active" data-target="about">Home</a>
                <a href="#experience" class="nav-link py-1 px-3 text-gray-700" data-target="experience">Experience</a>
                <a href="#education" class="nav-link py-1 px-3 text-gray-700" data-target="education">Education</a>
                <a href="#publications" class="nav-link py-1 px-3 text-gray-700" data-target="publications">Research</a>
                <a href="#skills" class="nav-link py-1 px-3 text-gray-700" data-target="skills">Skills</a>
                <a href="#extracurricular" class="nav-link py-1 px-3 text-gray-700" data-target="extracurricular">Activities</a>
                <a href="#gallery" class="nav-link py-1 px-3 text-gray-700" data-target="gallery">Gallery</a>
                <a href="#contact" class="nav-link py-1 px-3 text-gray-700" data-target="contact">Contact</a>
            </nav>
        </div>
    </header>

    <main class="flex-grow">
        <div class="container mx-auto px-6 py-4">
            
            <section id="about" class="content-section active">
                <div class="text-center md:flex md:items-center md:text-left">
                    <div class="md:w-1/3 flex justify-center mb-4 md:mb-0 md:mr-6">
                        <img src="https://placehold.co/200x200/0059B3/fff?text=Dr.+D.+Sushmitha" alt="Profile Picture" class="profile-picture w-36 h-36 md:w-48 md:h-48 object-cover">
                    </div>
                    <div class="md:w-2/3">
                        <h2 class="text-4xl md:text-5xl font-extrabold text-gray-900 leading-tight">Chemical Engineering Specialist</h2>
                        <h3 class="text-xl font-semibold mt-2 text-accent">Process Intensification, Biomass Valorisation & Academic Excellence</h3>
                        <p class="mt-3 text-gray-700 max-w-xl mx-auto md:mx-0 leading-relaxed text-base">
                            [cite_start]I leverage <span style="color: #FF007F;">over 10 years of experience</span> [cite: 4] across academia, research, and management. My core expertise is in <span style="color: #FF007F;">Sustainable Technology</span>, advanced coatings, and process modeling using <span style="color: #FF007F;">ASPEN</span> and <span style="color: #FF007F;">ANSYS</span>.
                        </p>
                        <div class="flex justify-center md:justify-start space-x-4 mt-4">
                            <a href="#experience" class="btn btn-projects text-sm" data-target="experience">View Career</a>
                            <a href="#contact" class="btn btn-contact text-sm" data-target="contact">Connect</a>
                        </div>
                    </div>
                </div>
            </section>

            <section id="experience" class="content-section">
                [cite_start]<h2 class="text-2xl font-bold section-heading">Professional Experience (10 Years, 7 Months) [cite: 4]</h2>
                <div class="grid md:grid-cols-2 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Asst. [cite_start]Professor (Temporary) [cite: 6]</h3>
                        <span class="text-gray-600 text-sm inline-block mr-2">Biotech, JNTU-H | [cite_start]Jan 2025 - Present. [cite: 6]</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Taught: <span style="color: #FF007F;">Process engineering principles</span>[cite: 8]. [cite_start]Labs: <span style="color: #FF007F;">Chemical Reaction Engineering Lab, Enzyme engineering Lab</span>[cite: 9].</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Business Development & Sales Manager [cite: 16]</h3>
                        <span class="text-gray-600 text-sm inline-block mr-2">Riss InfoTech | [cite_start]Jul - Aug 2023. [cite: 17]</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Managed CRM (<span style="color: #FF007F;">70 employees</span>)[cite: 18]. [cite_start]Executed <span style="color: #FF007F;">Digital marketing</span> [cite: 19][cite_start], <span style="color: #FF007F;">HR/Payroll</span>[cite: 22]. [cite_start]Acquired <span style="color: #FF007F;">Leadership skills</span>[cite: 19].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Asst. [cite_start]Professor & Coordinator [cite: 10]</h3>
                        <span class="text-gray-600 text-sm inline-block mr-2">Petrochemical Tech, Excel Engg College | [cite_start]May - Nov 2022. [cite: 11]</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Taught: <span style="color: #FF007F;">Electrochemistry, CRE I & II, Catalytic Engg, Fluid Mechanics</span>[cite: 12, 13, 14]. [cite_start]Roles: <span style="color: #FF007F;">Placement Co-ordinator, Hostel Warden, Class Advisor/Mentor, Internship Co-ordinator</span>[cite: 14, 15].</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Researcher (Ph.D. Scholar) [cite: 23]</h3>
                        <span class="text-gray-600 text-sm inline-block mr-2">NIT Warangal | [cite_start]May 2015 - Jul 2021. [cite: 23]</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Project: <span style="color: #FF007F;">Process Intensification (delignification)</span>[cite: 23]. [cite_start]Software: <span style="color: #FF007F;">ASPEN plus/Hysis, ANSYS (3D Modeling)</span>[cite: 23].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Asst. [cite_start]Professor [cite: 23]</h3>
                        <span class="text-gray-600 text-sm inline-block mr-2">Biotech, JNTU-H | [cite_start]Dec 2011 - Apr 2014. [cite: 23]</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Taught: <span style="color: #FF007F;">Process Engg Principles, Advanced transport phenomenon, Bioprocess Modelling, Bioprocess engineering principles, Basic engineering mathematics</span>[cite: 24, 25, 26, 27]. [cite_start]Managed labs[cite: 28].</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Industrial Training [cite: 29, 30, 32]</h3>
                        <span class="text-gray-600 text-sm inline-block mr-2">Vizag Steel, KERBS, Indo American Pharma | [cite_start]2007-2011. [cite: 29, 30, 32]</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Hands-on experience in equipment/processes and <span style="color: #FF007F;">Bulk Drug Production</span>[cite: 31, 32].</span>
                    </div>
                </div>
            </section>

            <section id="education" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Educational Qualifications</h2>
                <div class="grid md:grid-cols-2 gap-1">
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Ph.D. in Chemical Engineering [cite: 52]</h3>
                        <span class="text-gray-600 text-sm inline-block mr-2">NIT Warangal | [cite_start]Aug 2015 - Mar 2021. [cite: 52]</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Thesis: Acoustic Cavitation for <span style="color: #FF007F;">Self-Healing Corrosion Inhibition Coatings</span>[cite: 53].</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">M.Tech in Chemical Engineering (7.28 CGPA) [cite: 54]</h3>
                        <span class="text-gray-600 text-sm inline-block mr-2">NIT Warangal | [cite_start]Jul 2009 - Jul 2011. [cite: 55]</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Specialization: <span style="color: #FF007F;">Computer Aided Process Equipment Design</span>[cite: 55]. [cite_start]Thesis: Crude Benzol production using Aspen[cite: 55].</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">B.Tech in Chemical Engineering (67.56%) [cite: 56]</h3>
                        <span class="text-gray-600 text-sm inline-block mr-2">JNTU Anantapur | [cite_start]Jul 2004 - Jul 2008. [cite: 57]</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Thesis: Simulation of <span style="color: #FF007F;">large-scale membrane reformers</span> (two-dimensional model)[cite: 57].</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">GATE Qualification & Fellowships [cite: 48, 49, 50]</h3>
                        [cite_start]<span class="text-gray-600 text-sm inline-block mr-2">Qualified GATE <span style="color: #FF007F;">three times</span> (2009, 2010, 2012)[cite: 48]; [cite_start]Highest Rank: <span style="color: #FF007F;">1219</span>[cite: 60].</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Awarded <span style="color: #FF007F;">MHRD Scholarship</span> (Ph.D.) [cite: 49] [cite_start]and <span style="color: #FF007F;">AICTE Fellowship</span> (M.Tech)[cite: 50].</span>
                    </div>
                    <div class="card card-content md:col-span-2">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Pre-University and Schooling [cite: 58, 59]</h3>
                        [cite_start]<span class="text-gray-600 text-sm inline-block mr-2">Intermediate (M.P.C): 83.7% (Narayana). [cite: 58]</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Matriculation (SSC): 80.3% (St Mary's School). [cite: 59]</span>
                    </div>
                </div>
            </section>

            <section id="publications" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Research, Publications & Recognitions</h2>
                <div class="grid md:grid-cols-2 gap-1">
                    <div class="card card-content md:col-span-2">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Core Research Areas [cite: 35]</h3>
                        <span class="text-gray-700 text-sm"><span style="color: #FF007F;">Process Intensification</span>, Biorefinery, Biomass Valorisation, Paper Manufacturing, UV-Protective cloth, SAP, <span style="color: #FF007F;">Supercapacitors</span>, Dielectric paints, Conductive polymers, Hydrogel, Self-healing materials (corrosion/concrete).</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Publications & Output [cite: 101]</h3>
                        <ul class="horizontal-list text-gray-700 text-sm">
                            [cite_start]<li><span style="color: #FF007F;">6</span> Journal Papers (incl. *Ultrasonication and Sonochemistry*, IF: 9.336) [cite: 62]</li>
                            [cite_start]<li><span style="color: #FF007F;">19</span> Conference Papers (15 Intl, 4 Natl) [cite: 101]</li>
                            [cite_start]<li><span style="color: #FF007F;">2</span> Book Chapters [cite: 101]</li>
                        </ul>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Awards & Professional Roles [cite: 44, 46]</h3>
                        <ul class="horizontal-list text-gray-700 text-sm">
                            [cite_start]<li><span style="color: #FF007F;">Best Paper Award</span> (Research Conclave-17) [cite: 44]</li>
                            [cite_start]<li>Official Reviewer for <span style="color: #FF007F;">3 Elsevier journals</span> [cite: 46, 47]</li>
                            [cite_start]<li>Memberships: Associate Member of <span style="color: #FF007F;">IICHE</span> and <span style="color: #FF007F;">IEI</span> [cite: 51]</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <section id="skills" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Skills & Core Expertise</h2>
                <div class="grid md:grid-cols-2 gap-1">
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Software & Simulation [cite: 23]</h3>
                        <span class="text-gray-700 text-sm"><span style="color: #FF007F;">ASPEN plus, ASPEN tasc+, ASPEN Hysis</span>, ANSYS (3D Modeling), CRM Software.</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Experimental & Techniques [cite: 36]</h3>
                        <span class="text-gray-700 text-sm">Hydrodynamic / <span style="color: #FF007F;">Acoustic cavitation</span>, Polarization, <span style="color: #FF007F;">EIS</span> (electro chemical impedance spectroscopy), Equipment handling.</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Academic & Teaching [cite: 14, 15]</h3>
                        <span class="text-gray-700 text-sm">Curriculum Development, Class Advising, Mentoring, <span style="color: #FF007F;">Placement Coordination</span>, <span style="color: #FF007F;">Hostel Warden</span>, Internship Co-ordinator.</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Business & Management [cite: 16, 19, 22]</h3>
                        <span class="text-gray-700 text-sm"><span style="color: #FF007F;">Business Development</span>, Digital Marketing, Lead Generation, <span style="color: #FF007F;">HR/Payroll Management</span>.</span>
                    </div>
                </div>
            </section>

             <section id="extracurricular" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Extracurricular Activities & Honors</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Awards & Participation [cite: 123, 124, 129]</h3>
                        [cite_start]<span class="text-gray-700 text-sm inline-block mr-2">Sports: <span style="color: #FF007F;">First Prize in Running Race & Kho-kho</span> (JNTU-A, 2k7)[cite: 123, 124].</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block mr-2">Arts: <span style="color: #FF007F;">First Grade in All India Painting Competition</span> (Chennai)[cite: 129].</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Won <span style="color: #FF007F;">merit prize</span> in "Hindi Talent Test"[cite: 125].</span>
                    </div>
                    <div class="card card-content">
                         [cite_start]<h3 class="text-sm font-semibold text-gray-800">Seminars & Service [cite: 126, 127, 128, 102]</h3>
                        <span class="text-gray-700 text-sm inline-block mr-2">Participated in Intl. [cite_start]Symposiums <span style="color: #FF007F;">"FUSION-05" & "SCHEMCON-06"</span>[cite: 126].</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block mr-2">Bagged <span style="color: #FF007F;">National level certificate</span> for "All India Inter school cultural festival"[cite: 127].</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block mr-2"><span style="color: #FF007F;">Certified for collecting money for "Help age India"</span>[cite: 128].</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block">Assisted in <span style="color: #FF007F;">7 workshops</span>[cite: 102].</span>
                    </div>
                </div>
            </section>

            <section id="gallery" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Gallery (Professional & Academic Photos)</h2>
                <div class="grid md:grid-cols-3 gap-2">
                    <div class="card p-3">
                        <img src="https://placehold.co/400x300/0059B3/ffffff?text=Image+1+PLACEHOLDER" alt="Lab/Research Photo" class="gallery-image">
                        <p class="text-center text-sm text-gray-600 mt-2">Research work in the lab (Replace URL above).</p>
                    </div>
                    <div class="card p-3">
                        <img src="https://placehold.co/400x300/4CAF50/ffffff?text=Image+2+PLACEHOLDER" alt="Conference/Award Photo" class="gallery-image">
                        <p class="text-center text-sm text-gray-600 mt-2">Presenting at an International Conference (Replace URL above).</p>
                    </div>
                    <div class="card p-3">
                        <img src="https://placehold.co/400x300/FF5A5F/ffffff?text=Image+3+PLACEHOLDER" alt="Teaching/Group Photo" class="gallery-image">
                        <p class="text-center text-sm text-gray-600 mt-2">Group photo with students/colleagues (Replace URL above).</p>
                    </div>
                </div>
            </section>
            
            <section id="contact" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Contact & References</h2>
                <div class="grid md:grid-cols-2 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Contact Information</h3>
                        [cite_start]<span class="text-gray-700 text-sm inline-block mr-2">Phone: <span style="color: #FF007F;">7981541047 / 6304608610</span>[cite: 2].</span>
                        <span class="text-gray-700 text-sm inline-block">Email: <a href="mailto:Sushmitha.jntu@gmail.com" class="text-blue-600">Sushmitha.jntu@gmail.com</a> | [cite_start]<a href="mailto:sushmitha.d.nitw@gmail.com" class="text-blue-600">sushmitha.d.nitw@gmail.com</a>[cite: 3].</span>
                    </div>
                    <div class="card card-content">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">Online Research Profiles [cite: 37, 38]</h3>
                        [cite_start]<span class="text-gray-700 text-sm inline-block mr-2"><span style="color: #FF007F;">Google Scholar</span>: <a href="https://scholar.google.com/citations?user=Qk1uTQYAAAAJ" target="_blank" class="text-blue-600 hover:underline">View Profile</a>[cite: 37].</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block mr-2"><span style="color: #FF007F;">ORCID ID</span>: <a href="https://orcid.org/0000-0002-1125-6904" target="_blank" class="text-blue-600 hover:underline">0000-0002-1125-6904</a>[cite: 38].</span>
                        [cite_start]<span class="text-gray-700 text-sm inline-block"><span style="color: #FF007F;">Scopus ID</span>: 57213192955[cite: 38].</span>
                    </div>
                    <div class="card card-content md:col-span-2">
                        [cite_start]<h3 class="text-sm font-semibold text-gray-800">References (Available Upon Request) [cite: 105, 110, 113, 115]</h3>
                        <span class="text-gray-700 text-sm inline-block mr-2">Dr. S. Srinath (Assoc. Prof & Head, NIT-W) | Dr. Shirish Hari Sonawane (Prof, NIT-W) | Dr. K. Anand Kishore (Rtd Prof, NIT-W) | Dr. Pramod Kumar (Prof, JNTU-H).</span>
                    </div>
                </div>
            </section>

        </div>
    </main>

    <footer class="bg-white shadow-inner py-4 mt-4">
        <div class="container mx-auto px-6 text-center text-gray-600 text-sm">
            <p>&copy; 2023 All rights reserved.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const navLinks = document.querySelectorAll('.nav-link');
            const sections = document.querySelectorAll('.content-section');
            const projectButtons = document.querySelectorAll('[data-target]');
            
            const showSection = (targetId) => {
                sections.forEach(section => {
                    section.classList.remove('active');
                });
                const targetSection = document.getElementById(targetId);
                if (targetSection) {
                    targetSection.classList.add('active');
                }
            };

            const setActiveLink = (targetId) => {
                navLinks.forEach(link => {
                    link.classList.remove('active');
                });
                const activeLink = document.querySelector(`.nav-link[data-target="${targetId}"]`);
                if (activeLink) {
                    activeLink.classList.add('active');
                }
            };

            // Event listener for all interactive elements
            [...navLinks, ...projectButtons].forEach(element => {
                element.addEventListener('click', (e) => {
                    e.preventDefault();
                    const targetId = e.currentTarget.getAttribute('data-target');
                    showSection(targetId);
                    setActiveLink(targetId);
                    window.history.pushState(null, '', `#${targetId}`);
                });
            });

            // Handle initial load based on URL hash
            const initialSection = window.location.hash.substring(1) || 'about';
            showSection(initialSection);
            setActiveLink(initialSection);
        });
    </script>

</body>
</html>
