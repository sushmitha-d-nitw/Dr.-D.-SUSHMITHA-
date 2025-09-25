<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Resume | Specialist Portfolio</title>
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
            border: 6px solid #fff;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
        }
        /* Highly reduced card size for minimal space */
        .card {
            background-color: #ffffff;
            padding: 0.3rem 0.6rem; 
            border-radius: 4px;
            box-shadow: 0 1px 4px rgba(0, 0, 0, 0.04);
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            margin-bottom: 0.5rem; /* Reduced space between cards */
        }
        .card:hover {
            transform: translateY(-1px);
            box-shadow: 0 3px 8px rgba(0, 0, 0, 0.06);
        }
        .btn {
            padding: 0.5rem 1.5rem;
            border-radius: 9999px;
            font-weight: 600;
            transition: transform 0.2s ease;
        }
        .btn-projects { background-color: #FF5A5F; color: #fff; }
        .btn-contact { background-color: #4CAF50; color: #fff; }
        .text-accent { color: #2C7A7B; }
        .section-heading {
            border-bottom: 1px solid #e2e8f0;
            padding-bottom: 0.3rem;
            margin-bottom: 0.5rem;
            color: #1a202c;
        }
        .nav-link.active {
            color: #2C7A7B;
            font-weight: 700;
            border-bottom: 2px solid #2C7A7B;
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
            line-height: 1.2;
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
            margin-right: 8px;
            position: relative;
            padding-right: 8px;
        }
        .horizontal-list li:not(:last-child):after {
            content: "|";
            position: absolute;
            right: 0;
            color: #ccc;
        }
        .gallery-image {
            width: 100%;
            height: 150px;
            object-fit: cover;
            border-radius: 4px;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <header class="bg-white/80 backdrop-blur-sm shadow-sm py-3 sticky top-0 z-50">
        <div class="container mx-auto px-6 flex flex-col md:flex-row justify-between items-center">
            <h1 class="text-xl md:text-2xl font-bold">Chemical Engineering Portfolio</h1>
            <nav class="flex flex-wrap justify-center md:flex-row md:space-x-4 space-x-2 mt-2 md:mt-0 text-xs md:text-sm">
                <a href="#about" class="nav-link py-1 px-2 text-gray-600 active" data-target="about">Home</a>
                <a href="#experience" class="nav-link py-1 px-2 text-gray-600" data-target="experience">Experience</a>
                <a href="#education" class="nav-link py-1 px-2 text-gray-600" data-target="education">Education</a>
                <a href="#publications" class="nav-link py-1 px-2 text-gray-600" data-target="publications">Research</a>
                <a href="#skills" class="nav-link py-1 px-2 text-gray-600" data-target="skills">Skills</a>
                <a href="#extracurricular" class="nav-link py-1 px-2 text-gray-600" data-target="extracurricular">Activities</a>
                <a href="#gallery" class="nav-link py-1 px-2 text-gray-600" data-target="gallery">Gallery</a>
                <a href="#contact" class="nav-link py-1 px-2 text-gray-600" data-target="contact">Contact</a>
            </nav>
        </div>
    </header>

    <main class="flex-grow">
        <div class="container mx-auto px-6 py-4">
            
            <section id="about" class="content-section active">
                <div class="text-center md:flex md:items-center md:text-left">
                    <div class="md:w-1/3 flex justify-center mb-4 md:mb-0 md:mr-6">
                        <img src="https://placehold.co/200x200/2C7A7B/fff?text=Specialist" alt="Profile Picture" class="profile-picture w-32 h-32 md:w-40 md:h-40 object-cover">
                    </div>
                    <div class="md:w-2/3">
                        <h2 class="text-3xl md:text-4xl font-extrabold text-gray-900 leading-tight">Chemical Engineering Specialist</h2>
                        <h3 class="text-lg font-semibold mt-2 text-accent">Process Intensification, Biomass Valorisation & Academic Excellence</h3>
                        <p class="mt-2 text-gray-700 max-w-xl mx-auto md:mx-0 leading-relaxed text-sm">
                            I leverage **over 10 years of experience** across academia, research, and management. My core expertise is in **Sustainable Technology**, advanced coatings, and process modeling using **ASPEN** and **ANSYS**.
                        </p>
                        <div class="flex justify-center md:justify-start space-x-3 mt-3">
                            <a href="#experience" class="btn btn-projects text-xs" data-target="experience">View Career</a>
                            <a href="#contact" class="btn btn-contact text-xs" data-target="contact">Connect</a>
                        </div>
                    </div>
                </div>
            </section>

            <section id="experience" class="content-section">
                <h2 class="text-xl font-bold section-heading">Professional Experience (10 Years, 7 Months)</h2>
                <div class="grid md:grid-cols-2 gap-2">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Asst. Professor (Temporary)</h3>
                        <span class="text-gray-600 text-xs">Biotech, JNTU-H | Jan 2025 - Present.</span>
                        <span class="text-gray-700 text-xs">Taught **Process Engineering Principles**. Labs: CRE, Enzyme Engineering.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Business Development & Sales Manager</h3>
                        <span class="text-gray-600 text-xs">Riss InfoTech | Jul - Aug 2023.</span>
                        <span class="text-gray-700 text-xs">Managed **CRM (70 employees)**. Executed Digital Marketing, HR/Payroll.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Asst. Professor & Coordinator</h3>
                        <span class="text-gray-600 text-xs">Petrochemical Tech, Excel Engg College | May - Nov 2022.</span>
                        <span class="text-gray-700 text-xs">Taught **Electrochemistry, CRE I & II, Catalytic Engg, Fluid Mechanics**. Roles: Placement Co-ordinator, Hostel Warden.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Researcher (Ph.D. Scholar)</h3>
                        <span class="text-gray-600 text-xs">NIT Warangal | May 2015 - Jul 2021.</span>
                        <span class="text-gray-700 text-xs">Project: Process Intensification (delignification). Software: **ASPEN plus/Hysis, ANSYS (3D)**.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Asst. Professor</h3>
                        <span class="text-gray-600 text-xs">Biotech, JNTU-H | Dec 2011 - Apr 2014.</span>
                        <span class="text-gray-700 text-xs">Taught **Process Engg, Transport Phenomenon, Bioprocess Modelling**. Managed labs.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Industrial Training</h3>
                        <span class="text-gray-600 text-xs">Vizag Steel, KERBS, Indo American Pharma | 2007-2011.</span>
                        <span class="text-gray-700 text-xs">Hands-on experience in equipment, processes, and bulk drug production.</span>
                    </div>
                </div>
            </section>

            <section id="education" class="content-section">
                <h2 class="text-xl font-bold section-heading">Educational Qualifications</h2>
                <div class="grid md:grid-cols-2 gap-2">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Ph.D. in Chemical Engineering</h3>
                        <span class="text-gray-600 text-xs">NIT Warangal | Aug 2015 - Mar 2021.</span>
                        <span class="text-gray-700 text-xs">Thesis: Acoustic Cavitation for **Self-Healing Corrosion Inhibition Coatings**.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">M.Tech in Chemical Engineering (7.28 CGPA)</h3>
                        <span class="text-gray-600 text-xs">NIT Warangal | Jul 2009 - Jul 2011.</span>
                        <span class="text-gray-700 text-xs">Specialization: **Computer Aided Process Equipment Design**. Thesis: Crude Benzol production using Aspen.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">B.Tech in Chemical Engineering (67.56%)</h3>
                        <span class="text-gray-600 text-xs">JNTU Anantapur | Jul 2004 - Jul 2008.</span>
                        <span class="text-gray-700 text-xs">Thesis: Simulation of **large-scale membrane reformers** (two-dimensional model).</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">GATE Qualification & Fellowships</h3>
                        <span class="text-gray-600 text-xs">Qualified **GATE three times** (2009, 2010, 2012); Highest Rank: 1219.</span>
                        <span class="text-gray-700 text-xs">Awarded **MHRD Scholarship** (Ph.D.) and **AICTE Fellowship** (M.Tech).</span>
                    </div>
                    <div class="card card-content md:col-span-2">
                        <h3 class="text-sm font-semibold text-gray-800">Pre-University and Schooling</h3>
                        <span class="text-gray-600 text-xs">Intermediate (M.P.C): 83.7% (Narayana). Matriculation (SSC): 80.3% (St Mary's School).</span>
                    </div>
                </div>
            </section>

            <section id="publications" class="content-section">
                <h2 class="text-xl font-bold section-heading">Research, Publications & Recognitions</h2>
                <div class="grid md:grid-cols-2 gap-2">
                    <div class="card card-content md:col-span-2">
                        <h3 class="text-sm font-semibold text-gray-800">Core Research Areas</h3>
                        <span class="text-gray-700 text-xs">**Process Intensification**, Biorefinery, Biomass Valorisation, Paper Manufacturing, UV-Protective cloth, SAP, **Supercapacitors**, Dielectric paints, Conductive polymers, Hydrogel, Self-healing materials (corrosion/concrete).</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Publications & Output</h3>
                        <ul class="horizontal-list text-gray-700 text-xs">
                            <li>**6** Journal Papers (incl. *Ultrasonication and Sonochemistry*, IF: 9.336)</li>
                            <li>**19** Conference Papers (15 Intl, 4 Natl)</li>
                            <li>**2** Book Chapters</li>
                        </ul>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Awards & Professional Roles</h3>
                        <ul class="horizontal-list text-gray-700 text-xs">
                            <li>**Best Paper Award** (Research Conclave-17)</li>
                            <li>Official Reviewer for **3 Elsevier journals**</li>
                            <li>Memberships: Associate Member of **IICHE** and **IEI**</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <section id="skills" class="content-section">
                <h2 class="text-xl font-bold section-heading">Skills & Core Expertise</h2>
                <div class="grid md:grid-cols-2 gap-2">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Software & Simulation</h3>
                        <span class="text-gray-700 text-xs">**ASPEN plus, ASPEN tasc+, ASPEN Hysis**, ANSYS (3D Modeling), CRM Software.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Experimental & Techniques</h3>
                        <span class="text-gray-700 text-xs">Hydrodynamic / Acoustic cavitation, Polarization, EIS, Equipment handling.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Academic & Teaching</h3>
                        <span class="text-gray-700 text-xs">Curriculum Development, Class Advising, Mentoring, Placement Coordination, Hostel Warden.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Business & Management</h3>
                        <span class="text-gray-700 text-xs">Business Development, Digital Marketing, Lead Generation, HR/Payroll Management.</span>
                    </div>
                </div>
            </section>

             <section id="extracurricular" class="content-section">
                <h2 class="text-xl font-bold section-heading">Extracurricular Activities & Honors</h2>
                <div class="grid md:grid-cols-1 gap-2">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold text-gray-800">Awards & Participation</h3>
                        <span class="text-gray-700 text-xs">Sports: **First Prize in Running Race & Kho-kho** (JNTU-A, 2k7). Arts: **First Grade in All India Painting Competition** (Chennai). Won merit prize in **Hindi Talent Test**.</span>
                    </div>
                    <div class="card card-content">
                         <h3 class="text-sm font-semibold text-gray-800">Seminars & Service</h3>
                        <span class="text-gray-700 text-xs">Participated in Intl. Symposiums **"FUSION-05" & "SCHEMCON-06"**. Bagged Natl. certificate for **"All India Inter school cultural festival"**. Certified for collecting money for **"Help age India"**. Assisted in **7 workshops**.</span>
                    </div>
                </div>
            </section>

            <section id="gallery" class="content-section">
                <h2 class="text-xl font-bold section-heading">Gallery (Professional & Academic Photos)</h2>
                <div class="grid md:grid-cols-3 gap-4">
                    <div class="card p-2">
                        <img src="https://placehold.co/400x300/2C7A7B/ffffff?text=Image+1+Research+Lab" alt="Lab/Research Photo" class="gallery-image">
                        <p class="text-center text-xs text-gray-600 mt-1">Research work in the lab.</p>
                    </div>
                    <div class="card p-2">
                        <img src="https://placehold.co/400x300/4CAF50/ffffff?text=Image+2+Conference+Award" alt="Conference/Award Photo" class="gallery-image">
                        <p class="text-center text-xs text-gray-60
