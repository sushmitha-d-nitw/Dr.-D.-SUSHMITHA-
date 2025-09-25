<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dr. D. Sushmitha | Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f4f8;
            color: #333;
        }
        h1, h2 {
            font-family: 'Playfair Display', serif;
        }
        .container {
            max-width: 1200px;
        }
        .profile-picture {
            border-radius: 50%;
            border: 8px solid #fff;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
        }
        .card {
            background-color: #ffffff;
            /* Drastically reduced padding for minimal height */
            padding: 0.5rem 0.75rem; 
            border-radius: 6px;
            box-shadow: 0 1px 6px rgba(0, 0, 0, 0.04);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
        }
        .btn {
            padding: 0.6rem 1.8rem;
            border-radius: 9999px;
            font-weight: 600;
            transition: transform 0.2s ease;
        }
        .btn-projects { background-color: #FF5A5F; color: #fff; }
        .btn-contact { background-color: #4CAF50; color: #fff; }
        .text-accent { color: #2C7A7B; }
        .section-heading {
            border-bottom: 2px solid #e2e8f0;
            padding-bottom: 0.5rem;
            margin-bottom: 0.75rem; /* Reduced margin */
            color: #1a202c;
        }
        .nav-link.active {
            color: #2C7A7B;
            font-weight: 700;
            border-bottom: 2px solid #2C7A7B;
        }
        .content-section {
            display: none;
            animation: fadeIn 0.6s ease-in-out;
            /* Max height to ensure section content fits on screen */
            max-height: calc(100vh - 150px); 
            overflow-y: auto; 
            padding-right: 10px;
        }
        .content-section.active {
            display: block;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(5px); }
            to { opacity: 1; transform: translateY(0); }
        }
        /* Style for inner content lists to minimize space */
        .card ul {
            margin-top: 0.15rem;
        }
        .card ul li {
            margin-bottom: 0;
            line-height: 1.2;
        }
        .card h3 {
            margin-bottom: 0.1rem;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <header class="bg-white/80 backdrop-blur-sm shadow-sm py-3 sticky top-0 z-50">
        <div class="container mx-auto px-6 flex flex-col md:flex-row justify-between items-center">
            <h1 class="text-2xl font-bold">Dr. D. Sushmitha, Ph.D.</h1>
            <nav class="flex flex-wrap justify-center md:flex-row md:space-x-5 space-x-2 mt-3 md:mt-0 text-xs md:text-sm">
                <a href="#about" class="nav-link py-1 px-2 text-gray-600 active" data-target="about">Home</a>
                <a href="#experience" class="nav-link py-1 px-2 text-gray-600" data-target="experience">Experience</a>
                <a href="#education" class="nav-link py-1 px-2 text-gray-600" data-target="education">Education</a>
                <a href="#publications" class="nav-link py-1 px-2 text-gray-600" data-target="publications">Research</a>
                <a href="#skills" class="nav-link py-1 px-2 text-gray-600" data-target="skills">Skills</a>
                <a href="#extracurricular" class="nav-link py-1 px-2 text-gray-600" data-target="extracurricular">Activities</a>
                <a href="#contact" class="nav-link py-1 px-2 text-gray-600" data-target="contact">Contact</a>
            </nav>
        </div>
    </header>

    <main class="flex-grow">
        <div class="container mx-auto px-6 py-6">
            
            <section id="about" class="content-section active">
                <div class="text-center md:flex md:items-center md:text-left">
                    <div class="md:w-1/3 flex justify-center mb-5 md:mb-0 md:mr-8">
                        <img src="https://placehold.co/250x250/2C7A7B/fff?text=Dr.+Sushmitha" alt="Dr. D. Sushmitha" class="profile-picture w-36 h-36 md:w-48 md:h-48 object-cover">
                    </div>
                    <div class="md:w-2/3">
                        <h2 class="text-4xl md:text-5xl font-extrabold text-gray-900 leading-tight">Chemical Engineer & Academician</h2>
                        <h3 class="text-xl font-semibold mt-3 text-accent">Specialist in Process Intensification & Sustainable Tech</h3>
                        <p class="mt-3 text-gray-700 max-w-xl mx-auto md:mx-0 leading-relaxed text-sm">
                            I offer **over 10 years and 7 months** of combined experience across academia, industrial research, and management. My expertise drives innovation in **Process Intensification, Biomass Valorisation, Advanced Coatings**, and process modeling using tools like **ASPEN Hysis** and **ANSYS**.
                        </p>
                        <div class="flex justify-center md:justify-start space-x-3 mt-4">
                            <a href="#experience" class="btn btn-projects text-xs" data-target="experience">View Experience</a>
                            <a href="#contact" class="btn btn-contact text-xs" data-target="contact">Connect</a>
                        </div>
                    </div>
                </div>
            </section>

            <section id="experience" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Professional Experience (10+ Years)</h2>
                <div class="grid md:grid-cols-2 gap-3">
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Asst. Professor (Temporary)</h3>
                        <p class="text-gray-600 text-xs mt-0">Biotech, IST, JNTU-H | Jan 2025 - Present</p>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Teaching: Process Engineering Principles[cite: 8].</li>
                            <li>Labs: Chemical Reaction Engineering; [cite_start]Enzyme Engineering[cite: 9].</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Business Development & Sales Manager</h3>
                        <p class="text-gray-600 text-xs mt-0">Riss InfoTech | Jul 2023 - Aug 2023</p>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Managed 70 employees in CRM[cite: 18]. [cite_start]Digital marketing/Lead generation[cite: 19].</li>
                            <li>HR: Payroll generation; [cite_start]Department Allocation[cite: 22].</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Asst. Professor & Academic Coordinator</h3>
                        <p class="text-gray-600 text-xs mt-0">Petrochemical Tech, Excel Engg College | May - Nov 2022</p>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Courses: Electrochemistry [cite: 12][cite_start], CRE I & II [cite: 13, 14][cite_start], Catalytic Engg [cite: 13][cite_start], Fluid Mechanics[cite: 14].</li>
                            [cite_start]<li>Responsibilities: Placement Co-ordinator, Hostel Warden, Internship Co-ordinator[cite: 15].</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Researcher (Ph.D.)</h3>
                        <p class="text-gray-600 text-xs mt-0">NIT Warangal | May 2015 - Jul 2021</p>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Project: Process development for Intensification on delignification[cite: 23].</li>
                            [cite_start]<li>Software: ASPEN plus/tasc+/Hysis, ANSYS (3D Modeling)[cite: 23].</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Asst. Professor</h3>
                        <p class="text-gray-600 text-xs mt-0">Biotech, IST, JNTU-H | Dec 2011 - Apr 2014</p>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>M.Tech Courses: Process Engg. [cite: 24][cite_start], Advanced Transport Phenomenon [cite: 25][cite_start], Bioprocess Modelling[cite: 26], Basic Engg. [cite_start]Maths[cite: 27].</li>
                            <li>Labs Handled: Process Engg. Principles; [cite_start]Bioprocess Engg[cite: 28].</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Industrial Training</h3>
                        <p class="text-gray-600 text-xs mt-0">Vizag Steel Plant, KERBS, Indo American Pharma | 2007-2011</p>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Training on Equipment and Processes[cite: 31].</li>
                            [cite_start]<li>Training on Bulk Drug Production[cite: 32].</li>
                        </ul>
                    </div>
                </div>
            </section>

            <section id="education" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Educational Qualifications</h2>
                <div class="grid md:grid-cols-2 gap-3">
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Ph.D. in Chemical Engineering</h3>
                        <p class="text-gray-600 text-xs mt-0">NIT Warangal | Aug 2015 - Mar 2021</p>
                        [cite_start]<p class="mt-0 text-gray-700 text-xs">Thesis: Intensification of delignification by acoustic cavitation for self-healing corrosion inhibition coatings[cite: 53].</p>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">M.Tech in Chemical Engineering (7.28 CGPA)</h3>
                        <p class="text-gray-600 text-xs mt-0">NIT Warangal | Jul 2009 - Jul 2011</p>
                        [cite_start]<p class="mt-0 text-gray-700 text-xs">Specialization: Computer Aided Process Equipment Design[cite: 55]. [cite_start]Thesis: Improvement of crude benzol production using Aspen[cite: 55].</p>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">B.Tech in Chemical Engineering (67.56%)</h3>
                        <p class="text-gray-600 text-xs mt-0">JNTU Anantapur | Jul 2004 - Jul 2008</p>
                        [cite_start]<p class="mt-0 text-gray-700 text-xs">Thesis: Simulation of large-scale membrane reformers by a two-dimensional model[cite: 57].</p>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">GATE & Fellowships</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            <li>Qualified **GATE three times** (2009, 2010, 2012); [cite_start]Highest Rank: 1219[cite: 60, 48].</li>
                            [cite_start]<li>Received **MHRD Scholarship** (Ph.D.) and **AICTE Fellowship** (M.Tech)[cite: 49, 50].</li>
                        </ul>
                    </div>
                    <div class="card md:col-span-2">
                        <h3 class="text-sm font-semibold text-gray-800">Pre-University Qualifications</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Intermediate (M.P.C): 83.7% (Narayana Junior college)[cite: 58].</li>
                            [cite_start]<li>Matriculation (SSC): 80.3% (St Mary's School)[cite: 59].</li>
                        </ul>
                    </div>
                </div>
            </section>

            <section id="publications" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Research, Publications & Recognitions</h2>
                <div class="grid md:grid-cols-2 gap-3">
                    <div class="card md:col-span-2">
                        <h3 class="text-sm font-semibold text-gray-800">Research Focus Areas</h3>
                        [cite_start]<p class="mt-0 text-gray-700 text-xs">Process Intensification, Biorefinery, **Sustainable Biomass Valorisation** [cite: 35][cite_start], Paper manufacturing, UV-Protective cloth, Super Absorbent Polymer (SAP), Supercapacitors [cite: 33][cite_start], Dielectric paints, Conductive polymers, Hydrogel, Self-healing corrosion/concrete[cite: 35].</p>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Key Journal Publications (6 Total)</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>*Intensification of delignification...* - **Ultrasonication and Sonochemistry** (IF: 9.336)[cite: 62].</li>
                            [cite_start]<li>*Development of Ultrahigh build solid self-healing coatings...* - **Materials today Proceedings**[cite: 64].</li>
                            [cite_start]<li>*Thermal Modelling of a High Pressure Autoclave Reactor...* - **Lecture Notes in Mechanical Engineering**[cite: 66].</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Conferences, Chapters & Techniques</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Total: **15 International** & **4 National** Conference Papers[cite: 101]. [cite_start]**2 Book Chapters**[cite: 101].</li>
                            [cite_start]<li>Techniques: Hydrodynamic / Acoustic cavitation, Polarization, and EIS[cite: 36].</li>
                            [cite_start]<li>**Assisted 7 Workshops** and attended 9 GIAN Workshops[cite: 102, 103].</li>
                        </ul>
                    </div>
                    <div class="card md:col-span-2">
                        <h3 class="text-sm font-semibold text-gray-800">Awards & Professional Roles</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Recipient of the **Best Paper Award** at "Research Conclave-17," NIT Warangal (2017)[cite: 44, 45].</li>
                            [cite_start]<li>Official **Reviewer for three Elsevier journals**: *Renewable Energy* [cite: 46][cite_start], *Materials Today Proceedings* [cite: 46][cite_start], and *Journal of King Saud University*[cite: 47].</li>
                            [cite_start]<li>Memberships: Associate Member of **IICHE** (since 2017) and **IEI** (since 2023)[cite: 51].</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <section id="skills" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Skills & Core Expertise</h2>
                <div class="grid md:grid-cols-2 gap-3">
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Chemical Engineering Software</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>**Process Simulation:** ASPEN plus, ASPEN tasc+, ASPEN Hysis[cite: 23].</li>
                            [cite_start]<li>**Modeling:** ANSYS (3D Modeling)[cite: 23].</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Advanced Research Technologies</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>**New Energy:** Supercapacitors, Electrolytic Hydrogen Production[cite: 33].</li>
                            [cite_start]<li>**Polymer Chemistry:** Super Absorbent Polymer (SAP), Multifunctional Hydrogel[cite: 34].</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Academic & Teaching Proficiency</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Curriculum Planning, Mentoring, Class Committee Coordination[cite: 15].</li>
                            [cite_start]<li>Taught M.Tech/B.Tech subjects (10+ courses) and managed process/bioprocess labs[cite: 24, 28].</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Management & Business Skills</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Digital Marketing, Lead Generation, Client Scheduling[cite: 19, 21].</li>
                            [cite_start]<li>HR Functions: Payroll Generation, Department Allocation[cite: 22].</li>
                        </ul>
                    </div>
                </div>
            </section>

             <section id="extracurricular" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Extracurricular Activities & Honors</h2>
                <div class="grid md:grid-cols-2 gap-3">
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Sports & Arts Honors</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Won first prize in **Running Race** & **Kho-kho** (JNTU-A, 2k7)[cite: 123, 124].</li>
                            [cite_start]<li>Awarded **First Grade** in All India Painting Competition (Chennai)[cite: 129].</li>
                            [cite_start]<li>Won merit prize in **Hindi Talent Test** (Tenth class)[cite: 125].</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Participation & Service</h3>
                        <ul class="list-disc list-inside mt-0 text-gray-700 text-xs space-y-0">
                            [cite_start]<li>Certified for collecting money to **"Help age India"**[cite: 128].</li>
                            [cite_start]<li>Participated in Inter National level Symposium **"FUSION-05"** & **"SCHEMCON-06"**[cite: 126].</li>
                            [cite_start]<li>Bagged National level certificate for participating in **"All India Inter school cultural festival"**[cite: 127].</li>
                        </ul>
                    </div>
                </div>
            </section>

            <section id="contact" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Contact & References</h2>
                <div class="grid md:grid-cols-2 gap-3">
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Contact Information</h3>
                        <div class="mt-1 text-xs space-y-1">
                            [cite_start]<p><span class="font-semibold">Phone:</span> 7981541047 / 6304608610 [cite: 2]</p>
                            [cite_start]<p><span class="font-semibold">Email 1:</span> <a href="mailto:Sushmitha.jntu@gmail.com" class="text-blue-600">Sushmitha.jntu@gmail.com</a> [cite: 3]</p>
                            [cite_start]<p><span class="font-semibold">Email 2:</span> <a href="mailto:sushmitha.d.nitw@gmail.com" class="text-blue-600">sushmitha.d.nitw@gmail.com</a> [cite: 3]</p>
                        </div>
                    </div>
                    <div class="card">
                        <h3 class="text-sm font-semibold text-gray-800">Online Profiles</h3>
                        <div class="mt-1 text-xs space-y-1">
                            [cite_start]<p><span class="font-semibold">Google Scholar:</span> <a href="https://scholar.google.com/citations?user=Qk1uTQYAAAAJ" target="_blank" class="text-blue-600 hover:underline">View Profile</a> [cite: 37]</p>
                            [cite_start]<p><span class="font-semibold">ORCID ID:</span> <a href="https://orcid.org/0000-0002-1125-6904" target="_blank" class="text-blue-600 hover:underline">0000-0002-1125-6904</a> [cite: 38]</p>
                            [cite_start]<p><span class="font-semibold">Scopus ID:</span> 57213192955 [cite: 38]</p>
                        </div>
                    </div>
                    <div class="card md:col-span-2">
                        <h3 class="text-sm font-semibold text-gray-800">References (Available Upon Request)</h3>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Dr. [cite_start]S. Srinath (Associate Prof & Head, Chemical Engg, NIT-W)[cite: 105, 106, 119].</li>
                            <li>Dr. [cite_start]Shirish Hari Sonawane (Professor, Chemical Engg, NIT-W)[cite: 110, 119].</li>
                            <li>Dr. [cite_start]K. Anand Kishore (Rtd Professor, Chemical Engg, NIT-W)[cite: 113].</li>
                            <li>Dr. [cite_start]Pramod Kumar (Professor, Chemical Engg, CCST, IST, JNTU-H)[cite: 115, 117, 119].</li>
                        </ul>
                    </div>
                </div>
            </section>

        </div>
    </main>

    <footer class="bg-white shadow-inner py-3 mt-4">
        <div class="container mx-auto px-6 text-center text-gray-600 text-xs">
            <p>&copy; 2023 Dr. D. Sushmitha, Ph.D. All rights reserved.</p>
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

            // Event listener for navigation links and buttons (Home, Projects, Contact)
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
