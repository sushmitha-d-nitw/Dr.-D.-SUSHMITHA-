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
        .profile-picture {
            border-radius: 50%;
            border: 6px solid #fff;
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.2);
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
            background-color: #2A52BE; /* Kept this to ensure active section has a solid background */
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

    </style>
</head>
<body class="flex flex-col min-h-screen">

    <header class="shadow-md py-3 sticky top-0 z-50">
        <div class="container mx-auto px-4 md:px-2">
             <!-- The h1 for Dr. D. SUSHMITHA in white color was removed here -->
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
                        <img src="https://placehold.co/200x200/4285F4/fff?text=Dr.+D.+Sushmitha" alt="Profile Picture" class="profile-picture w-36 h-36 md:w-48 md:h-48 object-cover">
                    </div>
                    <div class="md:w-2/3">
                        <h2 class="text-4xl md:text-6xl font-extrabold leading-tight">Chemical Engineering Specialist</h2>
                        <h3 class="text-2xl font-semibold mt-2 text-accent">Process Intensification, Biomass Valorisation & Academic Excellence</h3>
                        <p class="mt-3 max-w-xl mx-auto md:mx-0 leading-relaxed text-base">
                            I leverage <span class="text-accent">over 10 years of experience</span> across academia, research, and management.
                            My core expertise is in <span class="text-accent">Sustainable Technology</span>, advanced coatings, and process modeling using <span class="text-accent">ASPEN</span> and <span class="text-accent">ANSYS</span>.
                        </p>
                        <div class="flex justify-center md:justify-start space-x-4 mt-4">
                            <a href="#experience" class="bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-2 px-4 rounded transition text-sm" data-target="experience">View Career</a>
                            <a href="#contact" class="bg-gray-200 hover:bg-gray-300 text-blue-900 font-bold py-2 px-4 rounded transition text-sm" data-target="contact">Connect</a>
                        </div>
                    </div>
                </div>
            </section>
            
            <section id="experience" class="content-section">
                <h2 class="section-heading">Professional Experience (10 Years, 7 Months)</h2>
                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-4">
                    <div class="card card-content">
                        <h3>Asst. Professor (Temporary)</h3>
                        <span class="text-sm font-semibold block">Biotech, JNTU-H | Jan 2025 - Present.</span>
                        <span class="text-sm block mt-1">Taught: <span class="text-accent">Process engineering principles</span>. Labs: <span class="text-accent">Chemical Reaction Engineering Lab, Enzyme engineering Lab</span>.</span>
                    </div>
                    <div class="card card-content">
                        <h3>Business Development & Sales Manager</h3>
                        <span class="text-sm font-semibold block">Riss InfoTech | Jul - Aug 2023.</span>
                        <span class="text-sm block mt-1">Managed CRM (<span class="text-accent">70 employees</span>). Executed <span class="text-accent">Digital marketing</span>, <span class="text-accent">HR/Payroll</span>. Acquired <span class="text-accent">Leadership skills</span>.</span>
                    </div>
                    <div class="card card-content">
                        <h3>Asst. Professor & Coordinator</h3>
                        <span class="text-sm font-semibold block">Petrochemical Tech, Excel Engg College | May - Nov 2022.</span>
                        <span class="text-sm block mt-1">Taught: <span class="text-accent">Electrochemistry, CRE I & II, Catalytic Engg, Fluid Mechanics</span>. Roles: <span class="text-accent">Placement Co-ordinator, Hostel Warden, Class Advisor/Mentor, Internship Co-ordinator</span>.</span>
                    </div>
                    <div class="card card-content">
                        <h3>Researcher (Ph.D. Scholar)</h3>
                        <span class="text-sm font-semibold block">NIT Warangal | May 2015 - Jul 2021.</span>
                        <span class="text-sm block mt-1">Project: <span class="text-accent">Process Intensification (delignification)</span>. Software: <span class="text-accent">ASPEN plus/Hysis, ANSYS (3D Modeling)</span>.</span>
                    </div>
                    <div class="card card-content">
                        <h3>Asst. Professor</h3>
                        <span class="text-sm font-semibold block">Biotech, JNTU-H | Dec 2011 - Apr 2014.</span>
                        <span class="text-sm block mt-1">Taught: <span class="text-accent">Process Engg Principles, Advanced transport phenomenon, Bioprocess Modelling, Bioprocess engineering principles, Basic engineering mathematics</span>. Managed labs.</span>
                    </div>
                    <div class="card card-content">
                        <h3>Industrial Training</h3>
                        <span class="text-sm font-semibold block">Vizag Steel Plant | 2010 - 2011</span>
                        <span class="text-sm block mt-1">Project: <span class="text-accent">Improvement of Crude Benzol Production</span>.</span>
                        <span class="text-sm font-semibold block mt-3">KERBS & Indo American Pharma | 2007</span>
                        <span class="text-sm block mt-1">Training: Hands-on experience in equipment/processes and <span class="text-accent">Bulk Drug Production</span>.</span>
                    </div>
                </div>
            </section>

            <section id="education" class="content-section">
                <h2 class="section-heading">Educational Qualifications</h2>
                <div class="grid md:grid-cols-2 gap-4">
                    <div class="card card-content">
                        <h3>Ph.D. in Chemical Engineering</h3>
                        <span class="text-sm font-semibold block">NIT Warangal | Aug 2015 - Mar 2021.</span>
                        <span class="text-sm block mt-1">Thesis: <span class="text-accent">Intensification of delignification from Tectona grandis by acoustic cavitation for development of self-healing corrosion inhibition coatings.</span></span>
                    </div>
                    <div class="card card-content">
                        <h3>M.Tech in Chemical Engineering (7.28 CGPA)</h3>
                        <span class="text-sm font-semibold block">NIT Warangal | Jul 2009 - Jul 2011.</span>
                        <span class="text-sm block mt-1">Specialization: <span class="text-accent">Computer Aided Process Equipment Design</span>.</span>
                        <span class="text-sm block mt-1">Project: <span class="text-accent">Improvement of Crude Benzol Production by Designing of 1-2 U-tube type Shell and Tube Heat Exchanger using Aspen.</span></span>
                    </div>
                    <div class="card card-content">
                        <h3>B.Tech in Chemical Engineering (67.56%)</h3>
                        <span class="text-sm font-semibold block">JNTU Anantapur | Jul 2004 - Jul 2008.</span>
                        <span class="text-sm block mt-1">Thesis: Simulation of <span class="text-accent">large-scale membrane reformers</span> (two-dimensional model).</span>
                    </div>
                    <div class="card card-content">
                        <h3>GATE Qualification & Fellowships</h3>
                        <span class="text-sm font-semibold block">Qualified GATE <span class="text-accent">three times</span> (2009, 2010, 2012); Highest Rank: <span class="text-accent">1219</span>.</span>
                        <span class="text-sm block mt-1">Awarded <span class="text-accent">MHRD Scholarship</span> (Ph.D.) and <span class="text-accent">AICTE Fellowship</span> (M.Tech).</span>
                    </div>
                </div>
            </section>

            <section id="research" class="content-section">
                <h2 class="section-heading">Core Research & Metrics</h2>
                <div class="grid md:grid-cols-2 gap-4">
                    <div class="card card-content md:col-span-2">
                        <h3>Core Research Areas</h3>
                        <span class="text-sm block mt-1"><span class="text-accent">Process Intensification</span>, Biorefinery, Biomass Valorisation, Paper Manufacturing, UV-Protective cloth, SAP, <span class="text-accent">Supercapacitors</span>, Dielectric paints, Conductive polymers, Hydrogel, Self-healing materials (corrosion/concrete).</span>
                    </div>
                    <div class="card card-content">
                        <h3>Publications & Output</h3>
                        <ul class="list-disc list-inside text-sm ml-4 space-y-1 mt-2">
                            <li><span class="text-accent">6</span> Journal Papers (incl. *Ultrasonication and Sonochemistry*, IF: 9.336)</li>
                            <li><span class="text-accent">15</span> International Conference Papers <span class="text-accent">(ISBNs added below)</span></li>
                            <li><span class="text-accent">2</span> Book Chapters</li>
                            <li><span class="text-accent">4</span> National Conference Papers</li>
                        </ul>
                    </div>
                    <div class="card card-content">
                        <h3>Awards & Professional Roles</h3>
                        <ul class="list-disc list-inside text-sm ml-4 space-y-1 mt-2">
                            <li><span class="text-accent">Best Paper Award</span> (Research Conclave-17)</li>
                            <li>Official Reviewer for <span class="text-accent">3 Elsevier journals</span></li>
                            <li>Memberships: Associate Member of <span class="text-accent">IICHE</span> and <span class="text-accent">IEI</span></li>
                        </ul>
                    </div>
                </div>
            </section>

            <section id="publications-detail" class="content-section">
                <h2 class="section-heading">Publications: Journals & Conferences</h2>
                <div class="card card-content">
                    
                    <h3>Journal Publications (6 Papers)</h3>
                    <ol class="list-decimal list-inside text-sm ml-4 mt-3 pub-list">
                        <li><span class="font-semibold text-accent">Intensification of delignification of Tectona grandis saw dust as sustainable biomass using acoustic cavitational devices.</span> in *Ultrasonication and Sonochemistry* (IF: 9.336, Indexed: SCI, Scopus). <a href="https://doi.org/10.1016/j.ultsonch.2019.104914" target="_blank" class="text-blue-300 hover:text-blue-100">[Original Paper]</a></li>
                        <li><span class="font-semibold text-accent">Development of Ultrahigh build solid self-healing coatings by silanized lignin Nano capsules.</span> in *Materials today Proceedings Journal*, Vol 45 (IF: 1.46, Indexed: Scopus). <a href="https://doi.org/10.1016/j.matpr.2021.02.576" target="_blank" class="text-blue-300 hover:text-blue-100">[Original Paper]</a></li>
                        <li><span class="font-semibold text-accent">Self-healing Corrosion Inhibition Coatings with PH-Responsive Activity by Incorporation of Nano Cellulose in Two pack epoxy polyamide system.</span> in *Materials today Proceedings Journal*, Vol 46 (IF: 1.46, Indexed: Scopus). <a href="https://doi.org/10.1016/j.matpr.2020.09.341" target="_blank" class="text-blue-300 hover:text-blue-100">[Original Paper]</a></li>
                        <li><span class="font-semibold text-accent">Thermal Modelling of a High Pressure Autoclave Reactor for Hydrothermal Carbonization.</span> in *Lecture Notes in Mechanical Engineering* (IF: 0.5, Indexed: Scopus). <a href="https://doi.org/10.1007/978-981-13-1903-763" target="_blank" class="text-blue-300 hover:text-blue-100">[Original Paper]</a></li>
                        <li><span class="font-semibold text-accent">Synthesis, and Characterization of Cellulose Nano fibers, in enhancing the tensile stress properties of paper composites.</span> in *International Journal of Engineering & Technology* (Indexed: Scopus H-Index: 2).</li>
                        <li><span class="font-semibold text-accent">Review on simulation of Heat Exchanger Using Aspen Plus Software.</span> in *International Journal of Emerging Trends in Engineering and development* (IF: 4.364, Indexed: Copernicus Index). <a href="http://www.rspublication.com/ijeted" target="_blank" class="text-blue-300 hover:text-blue-100">[Original Paper]</a></li>
                    </ol>

                    <h3 class="mt-6">International Conference Papers (15 Titles)</h3>
                    <ol class="list-decimal list-inside text-sm ml-4 mt-3 pub-list">
                        <li><span class="font-semibold text-accent">Synthesis of biodegradable multifunctional cellulose hydrogel produced from tectona grandis.</span> (RACEEE-2023) </li>
                        <li><span class="font-semibold text-accent">Comparison of self-healing performance of natural anti-corrosion agents, lignin and cellulose on mild steel.</span> (ICWEE-2021) </li>
                        <li><span class="font-semibold text-accent">Evolvement Of Electric Double Layer Pseudo Capacitor By Self-healing Corrosion Inhibition Of Mild Steel.</span> (SEMCON-2022) </li>
                        <li><span class="font-semibold text-accent">Review on Ultra high build solvent less self-healing coatings.</span> (2nd ICAMSE-2021) </li>
                        <li><span class="font-semibold text-accent">Comparison and Evaluation of corrosion inhibition performance of organic coatings.</span> (ICRAMC-2021) </li>
                        <li><span class="font-semibold text-accent">Lignin Encapsulation by Pickering Emulsion and In-Situ Polymerization for Corrosion Inhibition.</span> (EETSD-2020) <span class="isbn-highlight">ISBN: 978-93-86238-86-3</span></li>
                        <li><span class="font-semibold text-accent">Synthesis of Eco-Friendly and Multifunctional Lignin Based Cellulose Hydrogel from Tectona Grandis Sawdust.</span> (CRAFT 2020) </li>
                        <li><span class="font-semibold text-accent">Investigation of a controlled release rate studies on Benzotriazole Loaded Electrospun Cellulose hallow Nano Fibers.</span> (Nanotech 2019) <span class="isbn-highlight">ISBN: 978-93-82829-68-3</span></li>
                        <li><span class="font-semibold text-accent">Optimization of Hydrothermally treated sawdust using RSM CCD.</span> (INCEEE-2019) <span class="isbn-highlight">ISBN: 978-81-928314-5-9</span></li>
                        <li><span class="font-semibold text-accent">Intensification of enzyme activity using sonochemical approach.</span> (INCEEE-2019) <span class="isbn-highlight">ISBN: 978-81-928314-5-9</span></li>
                        <li><span class="font-semibold text-accent">Thermal Modelling of a high pressure Autoclave Reactor for Hydrothermal Carbonization.</span> (ICNHTFF-2018) <span class="isbn-highlight">ISBN: 2341-582</span></li>
                        <li><span class="font-semibold text-accent">Kinetic study of degradation of bagasse hydro char using Thermo gravimetric analysis.</span> (ICONSWM 2017) </li>
                        <li><span class="font-semibold text-accent">Microwave assisted alkali-peroxide treated sawdust for delignification and its characterization.</span> (ICONSWM 2017) </li>
                        <li><span class="font-semibold text-accent">Hydrothermal Carbonization of Waste Biomass.</span> (IHMTC2017) <span class="isbn-highlight">ISBN: 978-1-56700-478-6</span></li>
                        <li><span class="font-semibold text-accent">Early Research Work Title (15th Conference Paper) - Title not specified in source document.</span> (Placeholder)</li>
                    </ol>

                    <h3 class="mt-6">National Conference Papers (4)</h3>
                    <ul class="list-disc list-inside text-sm ml-4 mt-2">
                        <li>Optimization of Microwave assisted delignification process parameters... (RESEARCH CONCLAVE-2017), NITW, Warangal.</li>
                        <li>Ultrasound Assisted Pretreatment for efficient delignification of sawdust using sodium per carbonate. (CHEMCON-2016), IIT-Madras.</li>
                        <li>Simulation of large-scale membrane reformers by a two-dimensional model. (FUSION-07), JNTU A.</li>
                        <li>Supercritical extraction. (TECHNOZION-07), NIT-W.</li>
                    </ul>
                </div>
            </section>

            <section id="skills" class="content-section">
                <h2 class="section-heading">Skills & Core Expertise</h2>
                <div class="grid md:grid-cols-2 gap-4">
                    <div class="card card-content md:col-span-2">
                        <h3>Analytical & Spectroscopic Techniques</h3>
                        <p class="text-sm text-e0e0e0 italic mb-2">Techniques for identifying molecular structure and quantifying concentration.</p>
                        <div class="grid md:grid-cols-2 gap-x-6 text-sm">
                            <div>
                                <h4 class="sub-sub-heading">Spectroscopy Skills:</h4>
                                <ul class="list-disc list-inside ml-4 space-y-1 mt-1">
                                    <li><span class="font-semibold">Infrared (IR) & Raman Spectroscopy (FTIR & Raman):</span> Utilized for molecular identification, structural analysis, and polymorphism.</li>
                                    <li><span class="font-semibold">Nuclear Magnetic Resonance (NMR):</span> Expertise in determining precise molecular structure, purity, and concentration.</li>
                                    <li><span class="font-semibold">UV-Visible Spectrometry (UV-Vis):</span> Used for quantitative analysis and concentration determination.</li>
                                    <li><span class="font-semibold">Mass Spectrometry (MS):</span> Advanced skills in identifying unknown compounds and determining molecular weight and structure.</li>
                                </ul>
                            </div>
                            <div>
                                <h4 class="sub-sub-heading">Separation & Thermal Analysis:</h4>
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
                        <h3>Software & Simulation</h3>
                        <span class="text-sm"><span class="text-accent">ASPEN plus, ASPEN tasc+, ASPEN Hysis</span>, ANSYS (3D Modeling), CRM Software.</span>
                    </div>
                    <div class="card card-content">
                        <h3>Experimental & Techniques</h3>
                        <span class="text-sm">Hydrodynamic / <span class="text-accent">Acoustic cavitation</span>, Polarization, <span class="text-accent">EIS</span> (electro chemical impedance spectroscopy), Equipment handling.</span>
                    </div>
                </div>
            </section>

            <section id="extracurricular" class="content-section">
                <h2 class="section-heading">Extracurricular Activities & Honors</h2>
                <div class="grid md:grid-cols-1 gap-4">
                    <div class="card card-content">
                        <h3>Awards & Participation</h3>
                        <span class="text-sm block mt-1">Sports: <span class="text-accent">First Prize in Running Race & Kho-kho</span> (JNTU-A, 2k7).</span>
                        <span class="text-sm block mt-1">Academics: <span class="text-accent">Merit prize in "Hindi Talent Test"</span> and <span class="text-accent">Active participant in "FUSION-05" & "SCHEMCON-06"</span> events.</span>
                    </div>
                    <div class="card card-content">
                        <h3>Community & Other Honors</h3>
                        <span class="text-sm block mt-1">Received a certificate for actively collecting money for <span class="text-accent">"Help age India"</span>.</span>
                    </div>
                </div>
            </section>

            <section id="gallery" class="content-section">
                <h2 class="section-heading">Project Gallery & Research Visuals (10 Photos)</h2>
                <div class="grid grid-cols-2 lg:grid-cols-5 gap-3">
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
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/9C27B0/fff?text=Photo+5" alt="Gallery Image 5" class="gallery-image">
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/4CAF50/fff?text=Photo+6" alt="Gallery Image 6" class="gallery-image">
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/FFC107/fff?text=Photo+7" alt="Gallery Image 7" class="gallery-image">
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/03A9F4/fff?text=Photo+8" alt="Gallery Image 8" class="gallery-image">
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/E91E63/fff?text=Photo+9" alt="Gallery Image 9" class="gallery-image">
                    </div>
                    <div class="relative group">
                        <img src="https://placehold.co/400x300/9C27B0/fff?text=Photo+10" alt="Gallery Image 10" class="gallery-image">
                    </div>
                </div>
            </section>

            <section id="contact" class="content-section">
                <h2 class="section-heading">Contact & Professional Links</h2>
                <div class="card card-content">
                    <h3>Reach Out</h3>
                    <p class="text-sm mt-2 space-y-2">
                        <!-- Updated Contact Details -->
                        <span class="block">Email: <a href="mailto:sushmitha.d.nitw@gmail.com">sushmitha.d.nitw@gmail.com</a></span>
                        <span class="block">Phone: <span class="text-accent">+91 79815 41047</span></span>
                        
                        <!-- Added Professional IDs -->
<span class="block">LinkedIn: <a href="#linkedin" class="text-blue-300 hover:text-blue-100">linkedin.com/in/yourprofile</a></span>
<span class="block">Scopus ID: <span class="text-accent">57213192955</span>
<span class="block font-semibold">Google Scholar: <a href="[https://acesse.one/nuEPK]" class="text-blue-300 hover:text-blue-100">[GOOGLE SCHOLAR ID:Qk1uTQYAAAAJ]</a></span>
<span class="block font-semibold">ORCID ID: <a href="[https://orcid.org/0000-0002-1125-6904]">"class="text-blue-300 hover:text-blue-100">"[0000-0002-1125-6904]</a></span>
                    </p>
                </div>
            </section>

        </div>
    </main>

    <footer class="py-4 border-t border-white/20 mt-auto">
        <div class="container mx-auto px-6 text-center text-xs text-e0e0e0">
            <p>&copy; 2025 Dr. D. Sushmitha Portfolio. Designed with Tailwind CSS on a blue field.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const navLinks = document.querySelectorAll('.nav-link');
            const contentSections = document.querySelectorAll('.content-section');

            const showSection = (targetId) => {
                // Hide all sections
                contentSections.forEach(section => {
                    section.classList.remove('active');
                    section.style.display = 'none';
                });

                // Show the target section
                const targetSection = document.getElementById(targetId);
                if (targetSection) {
                    targetSection.style.display = 'block';
                    setTimeout(() => {
                        targetSection.classList.add('active');
                    }, 10);
                    
                    const mainContent = document.querySelector('main');
                    if (mainContent) {
                        mainContent.scrollTop = 0; 
                    }
                }
            };

            navLinks.forEach(link => {
                link.addEventListener('click', (e) => {
                    e.preventDefault();
                    const targetId = link.getAttribute('data-target');

                    // Update active nav link class
                    navLinks.forEach(nav => nav.classList.remove('active'));
                    link.classList.add('active');

                    showSection(targetId);
                });
            });

            // Initialize the page by showing the 'about' section on load
            const initialSection = document.querySelector('.nav-link.active');
            if (initialSection) {
                showSection(initialSection.getAttribute('data-target'));
            }
        });
    </script>

</body>
</html>
