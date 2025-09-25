<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Resume | Specialist Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        /* FINAL EXACT BLUE BACKGROUND: #2A52BE */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #2A52BE; 
            color: #ffffff; 
        }
        /* Ensure all structural elements have transparent backgrounds to show body blue */
        header, main, footer {
            background-color: transparent; 
        }

        h1, h2 {
            font-family: 'Playfair Display', serif;
            color: #ffffff; 
        }
        h3 {
            color: #ffffff; 
        }
        p, span, li {
            color: #e0e0e0; 
        }
        a {
            color: #90CAF9; 
        }
        a:hover {
            color: #BBDEFB;
        }

        .container {
            max-width: 1200px;
        }
        .profile-picture {
            border-radius: 50%;
            border: 6px solid #fff;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
        }
        /* Cards: Single column, minimal spacing */
        .card {
            background-color: rgba(255, 255, 255, 0.1); 
            padding: 0.3rem 0.6rem; 
            border-radius: 4px;
            box-shadow: 0 1px 4px rgba(0, 0, 0, 0.04);
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            margin-bottom: 0.5rem; /* Slightly more space for better separation in single column */
        }
        .card:hover {
            transform: translateY(-1px);
            box-shadow: 0 3px 8px rgba(0, 0, 0, 0.06);
        }
        /* Bright Yellow for high contrast highlights */
        .highlight { 
            color: #FFFF00; 
        } 
        .section-heading {
            border-bottom: 1px solid rgba(255, 255, 255, 0.2); 
            padding-bottom: 0.4rem;
            margin-bottom: 0.6rem;
            color: #ffffff; 
            font-size: 1.5rem; 
        }
        .nav-link {
            color: #ffffff; 
        }
        .nav-link.active {
            color: #FFFF00; 
            font-weight: 700;
            border-bottom: 2px solid #FFFF00;
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
        .card-content {
            display: flex;
            flex-direction: column;
            line-height: 1.3; 
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
            color: rgba(255, 255, 255, 0.3); 
        }
        .gallery-image {
            width: 100%;
            height: 180px; 
            object-fit: cover;
            border-radius: 4px;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        .detail-line {
            display: block;
            margin-top: 0.1rem;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <header class="shadow-sm py-3 sticky top-0 z-50">
        <div class="container mx-auto px-6 flex flex-col md:flex-row justify-end items-center">
            <h1 class="text-xl md:text-2xl font-bold"></h1> 
            <nav class="flex flex-wrap justify-center md:flex-row md:space-x-5 space-x-3 mt-2 md:mt-0 text-sm">
                <a href="#about" class="nav-link py-1 px-3 active" data-target="about">Home</a>
                <a href="#experience" class="nav-link py-1 px-3" data-target="experience">Experience</a>
                <a href="#education" class="nav-link py-1 px-3" data-target="education">Education</a>
                <a href="#awards" class="nav-link py-1 px-3" data-target="awards">Awards</a> <a href="#publications" class="nav-link py-1 px-3" data-target="publications">Research</a>
                <a href="#skills" class="nav-link py-1 px-3" data-target="skills">Skills</a>
                <a href="#extracurricular" class="nav-link py-1 px-3" data-target="extracurricular">Activities</a>
                <a href="#gallery" class="nav-link py-1 px-3" data-target="gallery">Gallery</a>
                <a href="#contact" class="nav-link py-1 px-3" data-target="contact">Contact</a>
            </nav>
        </div>
    </header>

    <main class="flex-grow">
        <div class="container mx-auto px-6 py-4">
            
            <section id="about" class="content-section active">
                <div class="text-center md:flex md:items-center md:text-left">
                    <div class="md:w-1/3 flex justify-center mb-4 md:mb-0 md:mr-6">
                        <img src="https://placehold.co/200x200/4285F4/fff?text=Dr.+D.+Sushmitha" alt="Profile Picture" class="profile-picture w-36 h-36 md:w-48 md:h-48 object-cover">
                    </div>
                    <div class="md:w-2/3">
                        <h2 class="text-4xl md:text-5xl font-extrabold leading-tight">Chemical Engineering Specialist</h2>
                        <h3 class="text-xl font-semibold mt-2 highlight">Process Intensification, Biomass Valorisation & Academic Excellence</h3>
                        <p class="mt-3 max-w-xl mx-auto md:mx-0 leading-relaxed text-base">
                            [cite_start]I leverage <span class="highlight">over 10 years 7 months of experience</span> across academia, research, and management[cite: 4]. [cite_start]My core expertise is in <span class="highlight">Sustainable Technology</span>, advanced coatings, and process modeling using <span class="highlight">ASPEN</span> and <span class="highlight">ANSYS</span>[cite: 23, 35].
                        </p>
                        <div class="flex justify-center md:justify-start space-x-4 mt-4">
                            <a href="#experience" class="btn btn-projects text-sm" data-target="experience">View Career</a>
                            <a href="#contact" class="btn btn-contact text-sm" data-target="contact">Connect</a>
                        </div>
                    </div>
                </div>
            </section>

            <section id="experience" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Professional Experience (10 Years, 7 Months)</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Asst. Professor (Temporary)</h3>
                        <span class="text-sm inline-block mr-2">Biotech, JNTU-H | [cite_start]<span class="highlight">Jan 2025 - Present</span>[cite: 6].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Batches: B.Tech 2nd year, M.Sc 2nd year Regular Batch[cite: 7].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Subjects taught: <span class="highlight">Process engineering principles</span>[cite: 8].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Labs: <span class="highlight">Chemical Reaction Engineering Lab, Enzyme engineering Lab</span>[cite: 9].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Asst. Professor & Coordinator</h3>
                        <span class="text-sm inline-block mr-2">Petrochemical Tech, Excel Engg College | [cite_start]<span class="highlight">May - Nov 2022</span>[cite: 11].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">B.Tech Courses taught: <span class="highlight">Electrochem. process tech (CE8091), CRE-I (PE8091), CRE-II (CE8601), Catalytic Engg (PE8072), Fluid mechanics (CH8301)</span>[cite: 12, 13, 14].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Academic Responsibilities: <span class="highlight">Placement Co-ordinator, Class Advisor/Mentor, Class committee Co-ordinator, Hostel Warden, Internship Co-ordinator</span>[cite: 14, 15].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Business Development & Sales Manager</h3>
                        <span class="text-sm inline-block mr-2">Riss InfoTech | [cite_start]<span class="highlight">Jul - Aug 2023</span>[cite: 17].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Manager Responsibilities: Maintaining <span class="highlight">70 employee data base in CRM</span>, <span class="highlight">Digital marketing for Lead generation</span>, Acquired <span class="highlight">Leadership skills</span>[cite: 18, 19].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Sales/HR Responsibilities: Scheduling Client meetings, Lead/Client information management in CRM, <span class="highlight">Pay roll generation</span>, Department Allocation[cite: 21, 22].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Researcher (Ph.D. Scholar)</h3>
                        <span class="text-sm inline-block mr-2">NIT Warangal | [cite_start]<span class="highlight">May 2015 - Jul 2021</span>[cite: 23].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Project Focus: Process development for <span class="highlight">Intensification on delignification</span>, Process Simulation, Optimization[cite: 23].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Software: <span class="highlight">ASPEN plus, ASPEN tasc+, ASPEN Hysis, ANSYS (3D Modeling)</span>[cite: 23].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Asst. Professor</h3>
                        <span class="text-sm inline-block mr-2">Biotech, JNTU-H | [cite_start]<span class="highlight">Dec 2011 - Apr 2014</span>[cite: 23].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">M.Tech Courses taught: <span class="highlight">Process Engg Principles, Advanced transport phenomenon, Bioprocess Modelling, Bioprocess engineering principles, Basic engineering mathematics</span>[cite: 24, 25, 26, 27].</span>
                        <span class="text-sm inline-block detail-line">Labs handled: Process engineering principles lab; [cite_start]Bioprocess engineering lab[cite: 28].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Industrial Training</h3>
                        [cite_start]<span class="text-sm inline-block mr-2"><span class="highlight">Vizag Steel Plant</span> (2010-2011), KERBS, Indo American Pharmaceuticals[cite: 29, 30, 32].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Training Focus: Equipment and Processes, <span class="highlight">Bulk Drug Production</span>[cite: 31, 32].</span>
                    </div>
                </div>
            </section>

            <section id="education" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Educational Qualifications</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Ph.D. in Chemical Engineering</h3>
                        <span class="text-sm inline-block mr-2">NIT Warangal | [cite_start]<span class="highlight">Aug 2015 - Mar 2021</span>[cite: 52].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Thesis: Intensification of delignification by acoustic cavitation for development of <span class="highlight">self-healing corrosion inhibition coatings</span>[cite: 53].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">M.Tech in Chemical Engineering (7.28 CGPA)</h3>
                        <span class="text-sm inline-block mr-2">NIT Warangal | [cite_start]<span class="highlight">Jul 2009 - Jul 2011</span>[cite: 54, 55].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Specialization: <span class="highlight">Computer Aided Process Equipment Design</span>[cite: 55].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Thesis: Improvement of crude benzol production by designing a 1-2 U-tube type shell and tube heat exchanger using Aspen[cite: 55].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">B.Tech in Chemical Engineering (67.56%)</h3>
                        <span class="text-sm inline-block mr-2">JNTU Anantapur | [cite_start]<span class="highlight">Jul 2004 - Jul 2008</span>[cite: 56, 57].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Thesis: Simulation of <span class="highlight">large-scale membrane reformers</span> by a two-dimensional model[cite: 57].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Pre-University and Schooling</h3>
                        [cite_start]<span class="text-sm inline-block mr-2">Intermediate (M.P.C): <span class="highlight">83.7%</span> (Narayana Junior college)[cite: 58].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Matriculation (SSC): <span class="highlight">80.3%</span> (St Mary's School)[cite: 59].</span>
                    </div>
                </div>
            </section>
            
            <section id="awards" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Awards and Recognition</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">GATE Qualification & Fellowships</h3>
                        [cite_start]<span class="text-sm inline-block mr-2">Qualified GATE <span class="highlight">three times</span> (2009, 2010, 2012)[cite: 48, 60]. [cite_start]Highest Rank: <span class="highlight">1219</span> (2009)[cite: 60].</span>
                        [cite_start]<span class="text-sm inline-block detail-line">Awarded <span class="highlight">MHRD Scholarship</span> (Ph.D.) and <span class="highlight">AICTE Fellowship</span> (M.Tech)[cite: 49, 50].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Academic Awards & Reviewer Roles</h3>
                        <ul class="horizontal-list text-sm">
                            [cite_start]<li><span class="highlight">Best Paper Award</span> at Research Conclave-17 (NITW, 2017)[cite: 44, 45].</li>
                            [cite_start]<li>Official Reviewer for <span class="highlight">3 Elsevier journals</span> (Renewable Energy, Materials Today Proceedings, Journal of King Saud University - Engineering Science)[cite: 46, 47].</li>
                        </ul>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Professional Memberships</h3>
                        <ul class="horizontal-list text-sm">
                            [cite_start]<li>Associate Member of <span class="highlight">IICHE</span> since Dec 2017[cite: 51].</li>
                            [cite_start]<li>Associate Member of <span class="highlight">IEI</span> (Institute of Engineers India) since Apr 2023[cite: 51].</li>
                        </ul>
                    </div>
                </div>
            </section>


            <section id="publications" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Research & Publications</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Research Output Summary</h3>
                        <ul class="horizontal-list text-sm">
                            [cite_start]<li><span class="highlight">6</span> Journal Papers [cite: 61, 101]</li>
                            [cite_start]<li><span class="highlight">2</span> Book Chapters [cite: 101]</li>
                            [cite_start]<li><span class="highlight">19</span> Conference Papers (15 Intl, 4 Natl) [cite: 101]</li>
                        </ul>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Core Research Areas</h3>
                        [cite_start]<span class="text-sm"><span class="highlight">Process Intensification, Biorefinery, Biomass Valorisation</span>, Paper Manufacturing, UV-Protective cloth, SAP, <span class="highlight">Supercapacitors</span>, Dielectric paints, Conductive polymers, Hydrogel, Self-healing corrosion/concrete[cite: 35].</span>
                        [cite_start]<span class="text-sm detail-line">Techniques: Hydrodynamic / <span class="highlight">Acoustic cavitation</span>, Polarization, <span class="highlight">EIS</span> (electro chemical impedance spectroscopy)[cite: 36].</span>
                    </div>
                </div>
            </section>
            
            <section id="skills" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Skills & Core Expertise</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Software & Simulation</h3>
                        [cite_start]<span class="text-sm"><span class="highlight">ASPEN plus, ASPEN tasc+, ASPEN Hysis</span>, ANSYS (3D Modeling), CRM Software[cite: 23, 18, 21].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Experimental & Techniques</h3>
                        [cite_start]<span class="text-sm">Hydrodynamic / <span class="highlight">Acoustic cavitation</span>, Polarization, <span class="highlight">EIS</span> (electro chemical impedance spectroscopy), Equipment handling[cite: 36, 31].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Academic & Teaching</h3>
                        [cite_start]<span class="text-sm">Curriculum Development, Class Advising, Mentoring, <span class="highlight">Placement Coordination</span>, <span class="highlight">Hostel Warden</span>, Internship Co-ordinator[cite: 14, 15].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Business & Management</h3>
                        [cite_start]<span class="text-sm"><span class="highlight">Business Development</span>, Digital Marketing, Lead Generation, <span class="highlight">HR/Payroll Management</span>[cite: 16, 19, 22].</span>
                    </div>
                </div>
            </section>

             <section id="extracurricular" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Extracurricular Activities & Honors</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Sports & Arts Achievements</h3>
                        <ul class="horizontal-list text-sm">
                            [cite_start]<li><span class="highlight">First Prize in Running Race & Kho-kho</span> (JNTU-A, 2k7)[cite: 123, 124].</li>
                            [cite_start]<li><span class="highlight">First Grade in All India Painting Competition</span> (Chennai)[cite: 129].</li>
                            [cite_start]<li>Won <span class="highlight">merit prize</span> in "Hindi Talent Test" (Tenth class)[cite: 125].</li>
                        </ul>
                    </div>
                    <div class="card card-content">
                         <h3 class="text-sm font-semibold">Seminars & Service</h3>
                        <ul class="horizontal-list text-sm">
                            <li>Participated in Intl. [cite_start]Symposiums <span class="highlight">"FUSION-05" & "SCHEMCON-06"</span>[cite: 126].</li>
                            [cite_start]<li>Bagged <span class="highlight">National level certificate</span> for "All India Inter school cultural festival"[cite: 127].</li>
                            [cite_start]<li><span class="highlight">Certified for collecting money for "Help age India"</span>[cite: 128].</li>
                            [cite_start]<li>Assisted for <span class="highlight">7 Workshops</span> for smooth running[cite: 102].</li>
                        </ul>
                    </div>
                </div>
            </section>

            <section id="gallery" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Gallery (Upload Your Photos)</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    <div class="card p-3">
                        <img src="https://placehold.co/800x250/4285F4/ffffff?text=Image+1+PLACEHOLDER" alt="Lab/Research Photo" class="gallery-image">
                        <p class="text-center text-sm mt-2">Research work in the lab (Replace URL/Base64 data in `src` attribute).</p>
                    </div>
                    <div class="card p-3">
                        <img src="https://placehold.co/800x250/4CAF50/ffffff?text=Image+2+PLACEHOLDER" alt="Conference/Award Photo" class="gallery-image">
                        <p class="text-center text-sm mt-2">Presenting at an International Conference (Replace URL/Base64 data in `src` attribute).</p>
                    </div>
                    <div class="card p-3">
                        <img src="https://placehold.co/800x250/FF5A5F/ffffff?text=Image+3+PLACEHOLDER" alt="Teaching/Group Photo" class="gallery-image">
                        <p class="text-center text-sm mt-2">Group photo with students/colleagues (Replace URL/Base64 data in `src` attribute).</p>
                    </div>
                </div>
            </section>
            
            <section id="contact" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Contact & References</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Contact Information</h3>
                        [cite_start]<span class="text-sm inline-block mr-2">Phone: <span class="highlight">7981541047 / 6304608610</span>[cite: 2].</span>
                        <span class="text-sm inline-block detail-line">Email: <a href="mailto:Sushmitha.jntu@gmail.com">Sushmitha.jntu@gmail.com</a> | [cite_start]<a href="mailto:sushmitha.d.nitw@gmail.com">sushmitha.d.nitw@gmail.com</a>[cite: 3].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Online Research Profiles</h3>
                        [cite_start]<span class="text-sm inline-block mr-2"><span class="highlight">Google Scholar</span>: <a href="https://scholar.google.com/citations?user=Qk1uTQYAAAAJ" target="_blank">View Profile</a>[cite: 37].</span>
                        [cite_start]<span class="text-sm inline-block detail-line"><span class="highlight">ORCID ID</span>: <a href="https://orcid.org/0000-0002-1125-6904" target="_blank">0000-0002-1125-6904</a>[cite: 38].</span>
                        [cite_start]<span class="text-sm inline-block detail-line"><span class="highlight">Scopus ID</span>: 57213192955[cite: 38].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">References (Available Upon Request)</h3>
                        <span class="text-sm detail-line">Dr. [cite_start]S. Srinath (Assoc. Prof & Head, NIT-W) [cite: 105, 106] | [cite_start]Dr. Shirish Hari Sonawane (Prof, NIT-W) [cite: 110] | [cite_start]Dr. K. Anand Kishore (Rtd Prof, NIT-W) [cite: 113] | [cite_start]Dr. Pramod Kumar (Prof, JNTU-H)[cite: 115].</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Declaration</h3>
                        [cite_start]<span class="text-sm">I hereby declare that the information furnished above is true to the best of my knowledge[cite: 131].</span>
                    </div>
                </div>
            </section>

        </div>
    </main>

    <footer class="shadow-inner py-4 mt-4">
        <div class="container mx-auto px-6 text-center text-sm">
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
