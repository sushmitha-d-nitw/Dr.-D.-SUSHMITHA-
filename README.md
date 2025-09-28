<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Resume | Specialist Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        /* FINAL EXACT BLUE BACKGROUND FROM IMAGE */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #2A52BE; /* Exact blue from the provided image */
            color: #ffffff; /* Default text color set to white for contrast */
        }
        /* Make header and main content background transparent/same as body for full blue effect */
        header, main, footer {
            background-color: transparent; 
        }

        h1, h2 {
            font-family: 'Playfair Display', serif;
            color: #ffffff; /* Ensure headings are white */
        }
        h3 {
            color: #ffffff; /* Ensure subheadings are white */
        }
        p, span, li {
            color: #e0e0e0; /* Lighter white for general text, slightly off-white */
        }
        a {
            color: #90CAF9; /* Light blue for links for visibility */
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
        /* Cards now have a slightly transparent white background to pop on blue */
        .card {
            background-color: rgba(255, 255, 255, 0.1); /* Slightly transparent white for cards */
            padding: 0.2rem 0.5rem;
            border-radius: 4px;
            box-shadow: 0 1px 4px rgba(0, 0, 0, 0.04);
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            margin-bottom: 0.3rem;
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
        .btn-projects { background-color: #FF5A5F; color: #fff; } /* Retain original btn colors for contrast */
        .btn-contact { background-color: #4CAF50; color: #fff; }
        .text-accent { color: #FFFF00; } /* Bright Yellow for accents to pop on blue */
        .section-heading {
            border-bottom: 1px solid rgba(255, 255, 255, 0.2); /* Lighter border for headings */
            padding-bottom: 0.4rem;
            margin-bottom: 0.6rem;
            color: #ffffff; 
            font-size: 1.5rem; 
        }
        .nav-link {
            color: #ffffff; /* Nav links white */
        }
        .nav-link.active {
            color: #FFFF00; /* Active nav link bright yellow */
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
            color: rgba(255, 255, 255, 0.3); /* Lighter separator for contrast */
        }
        .gallery-image {
            width: 100%;
            height: 180px; 
            object-fit: cover;
            border-radius: 4px;
            border: 1px solid rgba(255, 255, 255, 0.2);
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
                <a href="#research" class="nav-link py-1 px-3" data-target="research">Research</a>
                <a href="#publications-detail" class="nav-link py-1 px-3" data-target="publications-detail">Publications</a>
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
                        <h3 class="text-xl font-semibold mt-2 text-accent">Process Intensification, Biomass Valorisation & Academic Excellence</h3>
                        <p class="mt-3 max-w-xl mx-auto md:mx-0 leading-relaxed text-base">
                            I leverage <span style="color: #FFFF00;">over 10 years of experience</span> across academia, research, and management.
                            My core expertise is in <span style="color: #FFFF00;">Sustainable Technology</span>, advanced coatings, and process modeling using <span style="color: #FFFF00;">ASPEN</span> and <span style="color: #FFFF00;">ANSYS</span>.
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
                <div class="grid md:grid-cols-2 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Asst. Professor (Temporary)</h3>
                        <span class="text-sm inline-block mr-2">Biotech, JNTU-H | Jan 2025 - Present.</span>
                        <span class="text-sm inline-block">Taught: <span style="color: #FFFF00;">Process engineering principles</span>. Labs: <span style="color: #FFFF00;">Chemical Reaction Engineering Lab, Enzyme engineering Lab</span>.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Business Development & Sales Manager</h3>
                        <span class="text-sm inline-block mr-2">Riss InfoTech | Jul - Aug 2023.</span>
                        <span class="text-sm inline-block">Managed CRM (<span style="color: #FFFF00;">70 employees</span>). Executed <span style="color: #FFFF00;">Digital marketing</span>, <span style="color: #FFFF00;">HR/Payroll</span>. Acquired <span style="color: #FFFF00;">Leadership skills</span>.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Asst. Professor & Coordinator</h3>
                        <span class="text-sm inline-block mr-2">Petrochemical Tech, Excel Engg College | May - Nov 2022.</span>
                        <span class="text-sm inline-block">Taught: <span style="color: #FFFF00;">Electrochemistry, CRE I & II, Catalytic Engg, Fluid Mechanics</span>. Roles: <span style="color: #FFFF00;">Placement Co-ordinator, Hostel Warden, Class Advisor/Mentor, Internship Co-ordinator</span>.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Researcher (Ph.D. Scholar)</h3>
                        <span class="text-sm inline-block mr-2">NIT Warangal | May 2015 - Jul 2021.</span>
                        <span class="text-sm inline-block">Project: <span style="color: #FFFF00;">Process Intensification (delignification)</span>. Software: <span style="color: #FFFF00;">ASPEN plus/Hysis, ANSYS (3D Modeling)</span>.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Asst. Professor</h3>
                        <span class="text-sm inline-block mr-2">Biotech, JNTU-H | Dec 2011 - Apr 2014.</span>
                        <span class="text-sm inline-block">Taught: <span style="color: #FFFF00;">Process Engg Principles, Advanced transport phenomenon, Bioprocess Modelling, Bioprocess engineering principles, Basic engineering mathematics</span>. Managed labs.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Industrial Training</h3>
                        <span class="text-sm inline-block mr-2">Vizag Steel Plant | 2010 - 2011</span>
                        <span class="text-sm inline-block">Project: <span style="color: #FFFF00;">Improvement of Crude Benzol Production</span>.</span>
                        <span class="text-sm inline-block mr-2 mt-1">KERBS & Indo American Pharma | 2007</span>
                        <span class="text-sm inline-block">Training: Hands-on experience in equipment/processes and <span style="color: #FFFF00;">Bulk Drug Production</span>.</span>
                    </div>
                </div>
            </section>

            <section id="education" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Educational Qualifications</h2>
                <div class="grid md:grid-cols-2 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Ph.D. in Chemical Engineering</h3>
                        <span class="text-sm inline-block mr-2">NIT Warangal | Aug 2015 - Mar 2021.</span>
                        <span class="text-sm inline-block">Thesis: <span style="color: #FFFF00;">Intensification of delignification from Tectona grandis by acoustic cavitation for development of self-healing corrosion inhibition coatings.</span></span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">M.Tech in Chemical Engineering (7.28 CGPA)</h3>
                        <span class="text-sm inline-block mr-2">NIT Warangal | Jul 2009 - Jul 2011.</span>
                        <span class="text-sm inline-block">Specialization: <span style="color: #FFFF00;">Computer Aided Process Equipment Design</span>.</span>
                        <span class="text-sm inline-block">Project: <span style="color: #FFFF00;">Improvement of Crude Benzol Production by Designing of 1-2 U-tube Type Shell and Tube Heat Exchanger using Aspen.</span></span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">B.Tech in Chemical Engineering (67.56%)</h3>
                        <span class="text-sm inline-block mr-2">JNTU Anantapur | Jul 2004 - Jul 2008.</span>
                        <span class="text-sm inline-block">Thesis: Simulation of <span style="color: #FFFF00;">large-scale membrane reformers</span> (two-dimensional model).</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">GATE Qualification & Fellowships</h3>
                        <span class="text-sm inline-block mr-2">Qualified GATE <span style="color: #FFFF00;">three times</span> (2009, 2010, 2012); Highest Rank: <span style="color: #FFFF00;">1219</span>.</span>
                        <span class="text-sm inline-block">Awarded <span style="color: #FFFF00;">MHRD Scholarship</span> (Ph.D.) and <span style="color: #FFFF00;">AICTE Fellowship</span> (M.Tech).</span>
                    </div>
                    <div class="card card-content md:col-span-2">
                        <h3 class="text-sm font-semibold">Pre-University and Schooling</h3>
                        <span class="text-sm inline-block mr-2">Intermediate (M.P.C): 83.7% (Narayana).</span>
                        <span class="text-sm inline-block">Matriculation (SSC): 80.3% (St Mary's School).</span>
                    </div>
                </div>
            </section>

            <section id="research" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Core Research & Metrics</h2>
                <div class="grid md:grid-cols-2 gap-1">
                    <div class="card card-content md:col-span-2">
                        <h3 class="text-sm font-semibold">Core Research Areas</h3>
                        <span class="text-sm"><span style="color: #FFFF00;">Process Intensification</span>, Biorefinery, Biomass Valorisation, Paper Manufacturing, UV-Protective cloth, SAP, <span style="color: #FFFF00;">Supercapacitors</span>, Dielectric paints, Conductive polymers, Hydrogel, Self-healing materials (corrosion/concrete).</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Publications & Output</h3>
                        <ul class="horizontal-list text-sm">
                            <li><span style="color: #FFFF00;">6</span> Journal Papers (incl. *Ultrasonication and Sonochemistry*, IF: 9.336)</li>
                            <li><span style="color: #FFFF00;">19</span> Conference Papers (15 Intl, 4 Natl)</li>
                            <li><span style="color: #FFFF00;">2</span> Book Chapters</li>
                        </ul>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Awards & Professional Roles</h3>
                        <ul class="horizontal-list text-sm">
                            <li><span style="color: #FFFF00;">Best Paper Award</span> (Research Conclave-17)</li>
                            <li>Official Reviewer for <span style="color: #FFFF00;">3 Elsevier journals</span></li>
                            <li>Memberships: Associate Member of <span style="color: #FFFF00;">IICHE</span> and <span style="color: #FFFF00;">IEI</span></li>
                        </ul>
                    </div>
                </div>
            </section>

            <section id="publications-detail" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Publications: Journals & Conferences</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    
                    <div class="card card-content">
                        <h3 class="text-base font-bold">Journal Publications (6)</h3>
                        <ol class="list-decimal list-inside text-sm ml-4 mt-2 space-y-2">
                            <li><span class="font-semibold text-accent">Intensification of delignification from Tectona grandis...</span> in *Ultrasonication and Sonochemistry* (IF: 9.336, Indexed: SCI, Scopus). <a href="https://doi.org/10.1016/j.ultsonch.2019.104914" target="_blank" class="text-blue-300 hover:text-blue-100">Original Paper</a></li>
                            <li><span class="font-semibold text-accent">Development of Ultrahigh build solid self-healing coatings...</span> in *Materials today Proceedings Journal* (IF: 1.46, Indexed: Scopus). <a href="https://doi.org/10.1016/j.matpr.2021.02.576" target="_blank" class="text-blue-300 hover:text-blue-100">Original Paper</a></li>
                            <li><span class="font-semibold text-accent">Self-healing Corrosion Inhibition Coatings...</span> in *Materials today Proceedings Journal* (IF: 1.46, Indexed: Scopus). <a href="https://doi.org/10.1016/j.matpr.2020.09.341" target="_blank" class="text-blue-300 hover:text-blue-100">Original Paper</a></li>
                            <li><span class="font-semibold text-accent">Thermal Modelling of a High Pressure Autoclave Reactor...</span> in *Lecture Notes in Mechanical Engineering* (IF: 0.5, Indexed: Scopus). <a href="https://doi.org/10.1007/978-981-13-1903-763" target="_blank" class="text-blue-300 hover:text-blue-100">Original Paper</a></li>
                            <li><span class="font-semibold text-accent">Synthesis, and Characterization of Cellulose Nano fibers...</span> in *International Journal of Engineering & Technology* (Indexed: Scopus H-Indexed-2).</li>
                            <li><span class="font-semibold text-accent">Review on simulation of Heat Exchanger Using Aspen Plus Software</span> in *International Journal of Emerging Trends in Engineering and development* (IF: 4.364, Indexed: Copernicus Index). <a href="http://www.rspublication.com/ijeted" target="_blank" class="text-blue-300 hover:text-blue-100">Original Paper</a></li>
                        </ol>
                    </div>

                    <div class="card card-content">
                        <h3 class="text-base font-bold">International & National Conferences</h3>
                        <h4 class="text-sm font-semibold mt-2">International Conferences (5 of 15 listed)</h4>
                        <ul class="list-disc list-inside text-sm ml-4 space-y-1">
                            <li>"Synthesis of biodegradable multifunctional cellulose hydrogel..." (RACEEE-2023)</li>
                            <li>"Comparison of self-healing performance of natural anti-corrosion agents..." (ICWEE-2021)</li>
                            <li>"Evolvement Of Electric Double Layer Pseudo Capacitor..." (SEMCON-2022)</li>
                            <li>"Review on Ultra high build solvent less self-healing coatings" (ICAMSE-2021)</li>
                            <li>"Comparison and Evaluation of corrosion inhibition performance..." (ICRAMC-2021)</li>
                        </ul>
                        <h4 class="text-sm font-semibold mt-3">National Conferences (4)</h4>
                        <ul class="list-disc list-inside text-sm ml-4">
                            <li>Actively participated and presented papers at 4 national conferences.</li>
                            <li>Winner of the <span style="color: #FFFF00;">Best Paper Award</span> at Research Conclave-17.</li>
                        </ul>
                    </div>

                </div>
            </section>

            <section id="skills" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Skills & Core Expertise</h2>
                <div class="grid md:grid-cols-2 gap-1">

                    <div class="card card-content md:col-span-2">
                        <h3 class="text-sm font-semibold">Analytical & Spectroscopic Techniques</h3>
                        <p class="text-sm text-e0e0e0 italic mb-2">Techniques for identifying molecular structure and quantifying concentration.</p>
                        <div class="grid md:grid-cols-2 gap-x-6 text-sm">
                            <div>
                                <h4 class="font-bold text-accent">Spectroscopy Skills:</h4>
                                <ul class="list-disc list-inside ml-4 space-y-1 mt-1">
                                    <li><span class="font-semibold">Infrared (IR) & Raman Spectroscopy (FTIR & Raman):</span> Utilized for molecular identification, structural analysis, and polymorphism.</li>
                                    <li><span class="font-semibold">Nuclear Magnetic Resonance (NMR):</span> Expertise in determining precise molecular structure, purity, and concentration.</li>
                                    <li><span class="font-semibold">UV-Visible Spectrometry (UV-Vis):</span> Used for quantitative analysis and concentration determination.</li>
                                    <li><span class="font-semibold">Mass Spectrometry (MS):</span> Advanced skills in identifying unknown compounds and determining molecular weight and structure.</li>
                                </ul>
                            </div>
                            <div>
                                <h4 class="font-bold text-accent">Separation & Thermal Analysis:</h4>
                                <ul class="list-disc list-inside ml-4 space-y-1 mt-1">
                                    <li><span class="font-semibold">High-Performance Liquid Chromatography (HPLC):</span> Experienced in separating, purifying, and quantifying components in complex mixtures.</li>
                                    <li><span class="font-semibold">Thermo gravimetric Analysis (TGA):</span> Specialized in measuring thermal stability, decomposition kinetics, and material composition.</li>
                                    <li><span class="font-semibold">Particle Size Analyser:</span> Precision measurement of particle size distribution for quality control and formulation optimization.</li>
                                </ul>
                            </div>
                        </div>
                        <p class="text-sm text-e0e0e0 italic mt-3">Spectroscopy: (FTIR, Raman, NMR, UV-Vis, MS) These all interact with electromagnetic radiation (light or radio waves) to gather information about molecular structure and concentration.</p>
                    </div>

                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Software & Simulation</h3>
                        <span class="text-sm"><span style="color: #FFFF00;">ASPEN plus, ASPEN tasc+, ASPEN Hysis</span>, ANSYS (3D Modeling), CRM Software.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Experimental & Techniques</h3>
                        <span class="text-sm">Hydrodynamic / <span style="color: #FFFF00;">Acoustic cavitation</span>, Polarization, <span style="color: #FFFF00;">EIS</span> (electro chemical impedance spectroscopy), Equipment handling.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Academic & Teaching</h3>
                        <span class="text-sm">Curriculum Development, Class Advising, Mentoring, <span style="color: #FFFF00;">Placement Coordination</span>, <span style="color: #FFFF00;">Hostel Warden</span>, Internship Co-ordinator.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Business & Management</h3>
                        <span class="text-sm"><span style="color: #FFFF00;">Business Development</span>, Digital Marketing, Lead Generation, <span style="color: #FFFF00;">HR/Payroll Management</span>.</span>
                    </div>
                </div>
            </section>

            <section id="extracurricular" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Extracurricular Activities & Honors</h2>
                <div class="grid md:grid-cols-1 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Awards & Participation</h3>
                        <span class="text-sm inline-block mr-2">Sports: <span style="color: #FFFF00;">First Prize in Running Race & Kho-kho</span> (JNTU-A, 2k7).</span>
                        <span class="text-sm inline-block">Academics: <span style="color: #FFFF00;">Merit prize in "Hindi Talent Test"</span> and <span style="color: #FFFF00;">Active participant in "FUSION-05" & "SCHEMCON-06"</span> events.</span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Community & Other Honors</h3>
                        <span class="text-sm">Received a certificate for actively collecting money for <span style="color: #FFFF00;">"Help age India"</span>.</span>
                    </div>
                </div>
            </section>

            <section id="gallery" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Project Gallery & Research Visuals (10 Photos)</h2>
                <div class="grid grid-cols-2 md:grid-cols-5 gap-3">
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/4CAF50/fff?text=Photo+1" alt="Gallery Image 1" class="gallery-image">
                        <span class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity text-white text-xs p-2 text-center">Equipment Setup / Research Work</span>
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/FFC107/fff?text=Photo+2" alt="Gallery Image 2" class="gallery-image">
                        <span class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity text-white text-xs p-2 text-center">Lab Experiment</span>
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/03A9F4/fff?text=Photo+3" alt="Gallery Image 3" class="gallery-image">
                        <span class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity text-white text-xs p-2 text-center">Conference Presentation</span>
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/E91E63/fff?text=Photo+4" alt="Gallery Image 4" class="gallery-image">
                        <span class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity text-white text-xs p-2 text-center">Process Flow Diagram / Model</span>
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/9C27B0/fff?text=Photo+5" alt="Gallery Image 5" class="gallery-image">
                        <span class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity text-white text-xs p-2 text-center">Chemical Structure / Data Plot</span>
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/4CAF50/fff?text=Photo+6" alt="Gallery Image 6" class="gallery-image">
                        <span class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity text-white text-xs p-2 text-center">Equipment Setup / Research Work</span>
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/FFC107/fff?text=Photo+7" alt="Gallery Image 7" class="gallery-image">
                        <span class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity text-white text-xs p-2 text-center">Lab Experiment</span>
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/03A9F4/fff?text=Photo+8" alt="Gallery Image 8" class="gallery-image">
                        <span class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity text-white text-xs p-2 text-center">Conference Presentation</span>
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/E91E63/fff?text=Photo+9" alt="Gallery Image 9" class="gallery-image">
                        <span class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity text-white text-xs p-2 text-center">Process Flow Diagram / Model</span>
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/9C27B0/fff?text=Photo+10" alt="Gallery Image 10" class="gallery-image">
                        <span class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity text-white text-xs p-2 text-center">Chemical Structure / Data Plot</span>
                    </div>
                </div>
            </section>

            <section id="contact" class="content-section">
                <h2 class="text-2xl font-bold section-heading">Contact & Connect</h2>
                <div class="grid md:grid-cols-2 gap-1">
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Email & Phone</h3>
                        <span class="text-sm">Primary Email: <a href="mailto:Sushmitha.jntu@gmail.com">Sushmitha.jntu@gmail.com</a></span>
                        <span class="text-sm">Secondary Email: <a href="mailto:sushmitha.d.nitw@gmail.com">sushmitha.d.nitw@gmail.com</a></span>
                        <span class="text-sm">Contact: <span style="color: #FFFF00;">+91 7981541047 / 6304608610</span></span>
                    </div>
                    <div class="card card-content">
                        <h3 class="text-sm font-semibold">Online Profiles</h3>
                        <span class="text-sm">Google Scholar: <a href="https://scholar.google.com/citations?user=Qk1uTQYAAAAJ" target="_blank">View Profile</a></span>
                        <span class="text-sm">ORCID ID: <a href="https://orcid.org/0000-0002-1125-6904" target="_blank">0000-0002-1125-6904</a></span>
                    </div>
                </div>
            </section>

        </div>
    </main>

    <footer class="text-center py-4 text-sm mt-4">
        <div class="container mx-auto px-6">
            <p class="text-xs">Chemical Engineering Specialist Portfolio &copy; 2024</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const navLinks = document.querySelectorAll('.nav-link');
            const sections = document.querySelectorAll('.content-section');
            const projectButtons = document.querySelectorAll('.btn[data-target]');

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
