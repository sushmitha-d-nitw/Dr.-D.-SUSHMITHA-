<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Resume | Specialist Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Playfair+Display:wght=700&display=swap" rel="stylesheet">
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
            /* 1. REDUCED H3 FONT SIZE */
            font-size: 1.15rem; 
            line-height: 1.6rem;
            font-weight: 600;
            /* 2. REDUCED VERTICAL MARGIN BEFORE SUBHEADINGS */
            margin-bottom: 0.1rem; 
            margin-top: 0; 
            padding-top: 0;
        }

        /* Further reduce vertical margin before h3 inside publications-detail for tighter spacing */
        #publications-detail h3 {
             margin-top: 0.5rem; 
             margin-bottom: 0.1rem;
        }

        /* Sub-sub headings (H4/custom spans) */
        .sub-sub-heading {
            font-size: 1rem;
            line-height: 1.5rem;
            font-weight: 700;
            color: #FFFF00; /* Bright Yellow accent */
            margin-top: 0.5rem; /* Keep a little gap for these secondary headings */
            display: block;
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

        /* WIDENED CONTAINER MAX-WIDTH FOR MORE HORIZONTAL SPACE */
        .container {
            max-width: 1600px; 
        }
        
        /* ADJUSTED PROFILE PICTURE STYLES */
        .profile-picture {
            border-radius: 50%; /* Make it perfectly circular */
            border: 6px solid #fff;
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.2);
            width: 100%; 
            height: 100%; 
            object-fit: cover; 
        }
        .md\:w-1\/3 > .flex.justify-center {
            position: relative;
            width: 144px; 
            height: 144px; 
        }
        @media (min-width: 768px) { /* md breakpoint */
            .md\:w-1\/3 > .flex.justify-center {
                width: 192px; 
                height: 192px; 
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
            /* 3. INCREASED HORIZONTAL MARGIN/INDENTATION (left and right) */
            padding-left: 1.25rem !important; 
            padding-right: 1.25rem !important; 
            border-radius: 4px;
            transition: background-color 0.2s;
            white-space: nowrap; 
        }
        .nav-link.active {
            background-color: #4285F4;
            font-weight: 600;
        }
        
        /* --- START FIX FOR WIDER NAVIGATION BAR --- */
        
        /* 1. FORCE THE NAVIGATION BOX (The White Bar) TO BE WIDER */
        header .header-nav-container {
            /* Remove the Tailwind margin/padding around the nav bar to let it grow */
            padding-left: 0 !important;
            padding-right: 0 !important;
        }

        /* 2. TARGET THE <nav> ELEMENT AND SET A LARGE FIXED WIDTH */
        header nav {
            /* Set a generous fixed width to ensure ALL links (including Home/Contact) fit.
               You may need to slightly adjust 1250px depending on the screen size. */
            width: 1250px; 
            
            /* Center the wide nav bar visually */
            margin-left: auto;
            margin-right: auto;

            /* Crucial: Prevent the content from being clipped by the main viewport. 
               This will likely cause the entire page to show a horizontal scrollbar, 
               which is the necessary result of making an element wider than the screen. */
            overflow: visible !important; 
            
            /* Override the existing scroll behavior */
            overflow-x: hidden !important;
        }
        
        /* 3. Ensure the content container below the nav is also wide enough */
        main .container {
             max-width: 1250px; /* Match the nav width for layout consistency */
        }
        
        /* --- END FIX FOR WIDER NAVIGATION BAR --- */


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
            padding-bottom: 100%; 
            height: 0; 
            overflow: hidden; 
            border: 2px solid #fff; 
            box-sizing: border-box; 
        }
        .gallery-image { 
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover; 
            display: block;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <header class="shadow-md py-3 sticky top-0 z-50">
        <div class="container mx-auto px-4 md:px-2">
            </div>
        
        <div class="container mx-auto px-4 md:px-2 flex flex-col md:flex-row justify-center items-center header-nav-container">
            <nav class="flex justify-center md:space-x-1 space-x-2 mt-2 md:mt-0 text-sm"> 
                <a href="#about" class="nav-link active" data-target="about">Home</a>
                <a href="#experience" class="nav-link" data-target="experience">Experience</a>
                <a href="#education" class="nav-link" data-target="education">Education</a>
                <a href="#research" class="nav-link" data-target="research">Research</a>
                <a href="#publications-detail" class="nav-link" data-target="publications-detail">Publications</a>
                <a href="#skills" class="nav-link" data-target="skills">Skills</a>
                <a href="#extracurricular" class="nav-link" data-target="extracurricular">Awards & Recognition</a>
                <a href="#extra-curricular" class="nav-link" data-target="extra-curricular">Extra Curricular</a>
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
                        <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/refs/heads/main/website%20phototes/main%20.png" alt="Dr. D. Sushmitha Profile Picture" class="profile-picture w-36 h-36 md:w-48 md:h-48">
                    </div>
                    <div class="md:w-2/3">
                        <h2 class="text-3xl md:text-5xl font-extrabold leading-tight">Chemical Engineering Specialist</h2> 
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
                <div class="card card-content">
                    <ul class="list-disc list-inside text-sm ml-4 space-y-3 mt-3">
                        
                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Asst. Professor (Temporary)</span>
                                <span class="block">Biotech, JNTU-H | Jan 2025 - Present.</span>
                                <span class="block italic text-xs">Taught: <span class="text-accent">Process engineering principles</span>. Labs: <span class="text-accent">Chemical Reaction Engineering Lab, Enzyme engineering Lab</span>.</span>
                            </div>
                            <a href="files/experience_jntu_2025_proof.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Proof</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Business Development & Sales Manager</span>
                                <span class="block">Riss InfoTech | Jan - Aug 2023.</span>
                                <span class="block italic text-xs">Managed CRM (<span class="text-accent">70 employees</span>). Executed <span class="text-accent">Digital marketing</span>, <span class="text-accent">HR/Payroll</span>. Acquired <span class="text-accent">Leadership skills</span>.</span>
                            </div>
                            <a href="files/experience_riss_infotech_proof.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Proof</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Asst. Professor & Coordinator</span>
                                <span class="block">Petrochemical Tech, Excel Engg College | May - Nov 2022.</span>
                                <span class="block italic text-xs">Taught: <span class="text-accent">Electrochemistry, CRE I & II, Catalytic Engg, Fluid Mechanics</span>. Roles: <span class="text-accent">Placement Co-ordinator, Hostel Warden, Class Advisor/Mentor, Internship Co-ordinator</span>.</span>
                            </div>
                            <a href="files/experience_excel_proof.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Proof</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Researcher (Ph.D. Scholar)</span>
                                <span class="block">NIT Warangal | May 2015 - Jul 2021.</span>
                                <span class="block italic text-xs">Project: <span class="text-accent">Process Intensification (delignification)</span>. Software: <span class="text-accent">ASPEN plus/Hysis, ANSYS (3D Modeling)</span>.</span>
                            </div>
                            <a href="files/experience_nitw_research_proof.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Proof</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Asst. Professor</span>
                                <span class="block">Biotech, JNTU-H | Dec 2011 - Apr 2014.</span>
                                <span class="block italic text-xs">Taught: <span class="text-accent">Process Engg Principles, Advanced transport phenomenon, Bioprocess Modelling, Bioprocess engineering principles, Basic engineering mathematics</span>. Managed labs.</span>
                            </div>
                            <a href="files/experience_jntu_2011_proof.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Proof</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Industrial Training (Vizag Steel Plant)</span>
                                <span class="block">Vizag Steel Plant | 2010 - 2011.</span>
                                <span class="block italic text-xs">Project: <span class="text-accent">Improvement of Crude Benzol Production</span>.</span>

                                <span class="font-semibold text-accent block mt-3">Industrial Training (Pharma)</span>
                                <span class="block">KERBS & Indo American Pharma | 2007.</span>
                                <span class="block italic text-xs">Training: Hands-on experience in equipment/processes and <span class="text-accent">Bulk Drug Production</span>.</span>
                            </div>
                            <a href="files/experience_training_proof.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Proof</a>
                        </li>

                    </ul>
                </div>
            </section>
            <section id="education" class="content-section">
                <h2 class="section-heading">Educational Qualifications</h2>
                <div class="card card-content">
                    <ul class="list-disc list-inside text-sm ml-4 space-y-3 mt-3">
                        
                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Ph.D. in Chemical Engineering</span>
                                <span class="block">NIT Warangal | Aug 2015 - Mar 2021.</span>
                                <span class="block italic text-xs">Thesis: Intensification of delignification from Tectona grandis by acoustic cavitation for development of self-healing corrosion inhibition coatings.</span>
                            </div>
                            <a href="files/phd_certificate.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Certificate</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">M.Tech in Chemical Engineering (7.28 CGPA)</span>
                                <span class="block">NIT Warangal | Jul 2009 - Jul 2011.</span>
                                <span class="block italic text-xs">Specialization: Computer Aided Process Equipment Design. Project: Improvement of Crude Benzol Production...</span>
                            </div>
                            <a href="files/mtech_certificate.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Certificate</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">B.Tech in Chemical Engineering (67.56%)</span>
                                <span class="block">JNTU Anantapur | Jul 2004 - Jul 2008.</span>
                                <span class="block italic text-xs">Thesis: Simulation of large-scale membrane reformers (two-dimensional model).</span>
                            </div>
                            <a href="files/btech_certificate.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Certificate</a>
                        </li>
                        
                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Intermediate (Inter) - M.P.C. (Math's, Physics, Chemistry)</span>
                                <span class="block">83.7 % | 2002 - 2004.</span>
                                <span class="block italic text-xs">Narayana Junior college, Nellore, Andhra Pradesh.</span>
                            </div>
                            <a href="files/inter_certificate.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Certificate</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Matriculation (SSC Board)</span>
                                <span class="block">80.3 % | 2001 - 2002.</span>
                                <span class="block italic text-xs">St Mary’s School, Kavali, Nellore, Andhra Pradesh.</span>
                            </div>
                            <a href="files/matriculation_certificate.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Certificate</a>
                        </li>


                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">GATE Qualification & Fellowships</span>
                                <span class="block">Qualified GATE three times (2009, 2010, 2012); Highest Rank: 1219.</span>
                                <span class="block italic text-xs">Awarded MHRD Scholarship (Ph.D.) and AICTE Fellowship (M.Tech).</span>
                            </div>
                            <a href="files/gate_scorecard_certificate.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Certificate</a>
                        </li>
                    </ul>
                </div>
            </section>

            <section id="research" class="content-section">
                <h2 class="section-heading">Core Research & Metrics</h2>
                <div class="card card-content">
                    <ul class="list-disc list-inside text-sm ml-4 space-y-3 mt-3">
                        
                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Core Research Areas</span>
                                <span class="block italic text-xs">Expertise in: <span class="text-accent">Process Intensification</span>, Biorefinery, Biomass Valorisation, Paper Manufacturing, UV-Protective cloth, SAP, <span class="text-accent">Supercapacitors</span>, Dielectric paints, Conductive polymers, Hydrogel, Self-healing materials (corrosion/concrete).</span>
                            </div>
                            </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Publications & Output</span>
                                <span class="block mt-1">Output Summary:</span>
                                <ul class="list-circle list-inside ml-6 text-xs space-y-1 mt-1">
                                    <li><span class="text-accent">6</span> Journal Papers (incl. *Ultrasonication and Sonochemistry*, IF: 9.336)</li>
                                    <li><span class="text-accent">15</span> International Conference Papers</li>
                                    <li><span class="text-accent">2</span> Book Chapters; <span class="text-accent">4</span> National Conference Papers</li>
                                </ul>
                            </div>
                            </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Research & Professional Roles</span>
                                <span class="block mt-1">Professional Status:</span>
                                <ul class="list-circle list-inside ml-6 text-xs space-y-1 mt-1">
                                    <li>Official Reviewer for <span class="text-accent">3 Elsevier journals</span> (Details in Awards section).</li>
                                    <li>Memberships: Associate Member of <span class="text-accent">IICHE</span> and <span class="text-accent">IEI</span>.</li>
                                </ul>
                            </div>
                            </li>
                        
                    </ul>
                </div>
            </section>
            <section id="publications-detail" class="content-section">
                <h2 class="section-heading">Publications: Journals & Conferences</h2>
                <div class="card card-content">
                    
                    <h3>Journal Publications (6 Papers)</h3>
                    <ol class="list-decimal list-inside text-sm ml-4 mt-3 pub-list">
                        <li><span class="font-semibold">Intensification of delignification of Tectona grandis saw dust as sustainable biomass using acoustic cavitational devices.</span> in *Ultrasonication and Sonochemistry* (IF: 9.336, Indexed: SCI, Scopus). <a href="https://doi.org/10.1016/j.ultsonch.2019.104914" target="_blank" class="text-blue-300 hover:text-blue-100">[Original Paper]</a></li>
                        <li><span class="font-semibold">Development of Ultrahigh build solid self-healing coatings by silanized lignin Nano capsules.</span> in *Materials today Proceedings Journal*, Vol 45 (IF: 1.46, Indexed: Scopus). <a href="https://doi.org/10.1016/j.matpr.2021.02.576" target="_blank" class="text-blue-300 hover:text-blue-100">[Original Paper]</a></li>
                        <li><span class="font-semibold">Self-healing Corrosion Inhibition Coatings with PH-Responsive Activity by Incorporation of Nano Cellulose in Two pack epoxy polyamide system.</span> in *Materials today Proceedings Journal*, Vol 46 (IF: 1.46, Indexed: Scopus). <a href="https://doi.org/10.1016/j.matpr.2020.09.341" target="_blank" class="text-blue-300 hover:text-blue-100">[Original Paper]</a></li>
                        <li><span class="font-semibold">Thermal Modelling of a High Pressure Autoclave Reactor for Hydrothermal Carbonization.</span> in *Lecture Notes in Mechanical Engineering* (IF: 0.5, Indexed: Scopus). <a href="https://doi.org/10.1007/978-981-13-1903-763" target="_blank" class="text-blue-300 hover:text-blue-100">[Original Paper]</a></li>
                        <li><span class="font-semibold">Synthesis, and Characterization of Cellulose Nano fibers, in enhancing the tensile stress properties of paper composites.</span> in *International Journal of Engineering & Technology* (Indexed: Scopus H-Index: 2).</li>
                        <li><span class="font-semibold">Review on simulation of Heat Exchanger Using Aspen Plus Software.</span> in *International Journal of Emerging Trends in Engineering and development* (IF: 4.364, Indexed: Copernicus Index). <a href="http://www.rspublication.com/ijeted" target="_blank" class="text-blue-300 hover:text-blue-100">[Original Paper]</a></li>
                    </ol>

                    <h3 class="mt-6">International Conference Papers (15 Titles)</h3>
                    <ol class="list-decimal list-inside text-sm ml-4 mt-3 pub-list">
                        <li><span class="font-semibold">Synthesis of biodegradable multifunctional cellulose hydrogel produced from tectona grandis.</span> (RACEEE-2023) </li>
                        <li><span class="font-semibold">Comparison of self-healing performance of natural anti-corrosion agents, lignin and cellulose on mild steel.</span> (ICWEE-2021) </li>
                        <li><span class="font-semibold">Evolvement Of Electric Double Layer Pseudo Capacitor By Self-healing Corrosion Inhibition Of Mild Steel.</span> (SEMCON-2022) </li>
                        <li><span class="font-semibold">Review on Ultra high build solvent less self-healing coatings.</span> (2nd ICAMSE-2021) </li>
                        <li><span class="font-semibold">Comparison and Evaluation of corrosion inhibition performance of organic coatings.</span> (ICRAMC-2021) </li>
                        <li><span class="font-semibold">Lignin Encapsulation by Pickering Emulsion and In-Situ Polymerization for Corrosion Inhibition.</span> (EETSD-2020) <span class="isbn-highlight">ISBN: 978-93-86238-86-3</span></li>
                        <li><span class="font-semibold">Synthesis of Eco-Friendly and Multifunctional Lignin Based Cellulose Hydrogel from Tectona Grandis Sawdust.</span> (CRAFT 2020) </li>
                        <li><span class="font-semibold">Investigation of a controlled release rate studies on Benzotriazole Loaded Electrospun Cellulose hallow Nano Fibers.</span> (Nanotech 2019) <span class="isbn-highlight">ISBN: 978-93-82829-68-3</span></li>
                        <li><span class="font-semibold">Optimization of Hydrothermally treated sawdust using RSM CCD.</span> (INCEEE-2019) <span class="isbn-highlight">ISBN: 978-81-928314-5-9</span></li>
                        <li><span class="font-semibold">Intensification of enzyme activity using sonochemical approach.</span> (INCEEE-2019) <span class="isbn-highlight">ISBN: 978-81-928314-5-9</span></li>
                        <li><span class="font-semibold">Thermal Modelling of a high pressure Autoclave Reactor for Hydrothermal Carbonization.</span> (ICNHTFF-2018) <span class="isbn-highlight">ISBN: 2341-582</span></li>
                        <li><span class="font-semibold">Kinetic study of degradation of bagasse hydro char using Thermo gravimetric analysis.</span> (ICONSWM 2017) </li>
                        <li><span class="font-semibold">Microwave assisted alkali-peroxide treated sawdust for delignification and its characterization.</span> (ICONSWM 2017) </li>
                        <li><span class="font-semibold">Hydrothermal Carbonization of Waste Biomass.</span> (IHMTC2017) <span class="isbn-highlight">ISBN: 978-1-56700-478-6</span></li>
                        <li><span class="font-semibold">Early Research Work Title (15th Conference Paper) - Title not specified in source document.</span> (Placeholder)</li>
                    </ol>

                    <h3 class="mt-6">National Conference Papers (4)</h3>
                    <ul class="list-disc list-inside text-sm ml-4 mt-2">
                        <li>Optimization of Microwave assisted delignification process parameters... (RESEARCH CONCLAVE-2017), NITW, Warangal.</li>
                        <li>Ultrasound Assisted Pretreatment for efficient delignification of sawdust using sodium per carbonate. (CHEMCON-2016), IIT-Madras.</li>
                        <li>Simulation of large-scale membrane reformers by a two-dimensional model. (FUSION-07), JNTU-A.</li>
                        <li>Modelling of a high pressure... (Placeholder for 4th title).</li>
                    </ul>
                </div>
            </section>
            
            <section id="skills" class="content-section">
                <h2 class="section-heading">Technical & Professional Skills</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                    
                    <div class="card">
                        <h3>Domain Expertise</h3>
                        <ul class="list-disc list-inside ml-4 space-y-1 text-sm">
                            <li>Process Intensification (Acoustic Cavitation, Microwave)</li>
                            <li>Biomass Valorisation (Lignin, Cellulose, Hydrochar)</li>
                            <li>Advanced Coatings (Self-healing, Anti-corrosion)</li>
                            <li>Reaction & Transport Phenomena</li>
                            <li>Polymer & Nanomaterials Synthesis</li>
                        </ul>
                    </div>
                    
                    <div class="card">
                        <h3>Simulation & Software</h3>
                        <ul class="list-disc list-inside ml-4 space-y-1 text-sm">
                            <li><span class="font-semibold text-accent">ASPEN Plus/Hysis</span> (Process Flow Sheet & Simulation)</li>
                            <li><span class="font-semibold text-accent">ANSYS</span> (CFD Modeling & Simulation)</li>
                            <li>Design Expert (RSM, DOE)</li>
                            <li>MATLAB (Programming & Modeling)</li>
                            <li>MS Office Suite & Data Analysis</li>
                        </ul>
                    </div>
                    
                    <div class="card">
                        <h3>Laboratory Proficiency</h3>
                        <ul class="list-disc list-inside ml-4 space-y-1 text-sm">
                            <li>Spectroscopy (FTIR, UV-Vis, X-Ray)</li>
                            <li>Thermal Analysis (TGA, DSC)</li>
                            <li>Microscopy (SEM, TEM, AFM)</li>
                            <li>Surface Analysis (Contact Angle, Potentiostat/Galvanostat)</li>
                            <li>Process Equipment Operation</li>
                        </ul>
                    </div>
                    
                    <div class="card">
                        <h3>Management & Soft Skills</h3>
                        <ul class="list-disc list-inside ml-4 space-y-1 text-sm">
                            <li>Team Leadership & Mentoring (B.Tech/M.Tech)</li>
                            <li>Placement & Training Coordination</li>
                            <li>Client Relationship Management (CRM)</li>
                            <li>Technical Writing & Presentation</li>
                            <li>Digital Marketing & HR/Payroll Management</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <section id="extracurricular" class="content-section">
                <h2 class="section-heading">Awards & Recognition</h2>
                <div class="card card-content">
                    <ul class="list-disc list-inside text-sm ml-4 space-y-3 mt-3">

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Reviewer Recognition (Elsevier)</span>
                                <span class="block">Official Reviewer for the following Elsevier Journals:</span>
                                <ul class="list-circle list-inside ml-6 text-xs space-y-1 mt-1">
                                    <li>*International Journal of Biological Macromolecules* (IF: 8.2)</li>
                                    <li>*Separation Science and Technology* (IF: 2.3)</li>
                                    <li>*Materials Today Proceedings* (IF: 1.46)</li>
                                </ul>
                            </div>
                            <a href="files/reviewer_recognition.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Proof</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">National Level Award (Best Paper)</span>
                                <span class="block">Awarded Best Paper at the National Level Conference, CHEMCON (2016), IIT-Madras.</span>
                                <span class="block italic text-xs">For the paper: Ultrasound Assisted Pretreatment for efficient delignification of sawdust...</span>
                            </div>
                            <a href="files/best_paper_award.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Proof</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Academic Fellowships</span>
                                <span class="block">AICTE Fellowship for M.Tech, and MHRD Scholarship for Ph.D.</span>
                                <span class="block italic text-xs">Recognizing merit and excellence in post-graduate and doctoral studies.</span>
                            </div>
                            <a href="files/fellowship_proof.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Proof</a>
                        </li>

                        <li class="flex justify-between items-start pr-4">
                            <div class="flex-grow">
                                <span class="font-semibold text-accent block">Teaching & Student Mentoring Awards</span>
                                <span class="block">Multiple internal college recognitions for effective teaching and student guidance.</span>
                                <span class="block italic text-xs">Focused on mentoring students for projects, career choices, and personal development.</span>
                            </div>
                            </li>
                    </ul>
                </div>
            </section>
            
            <section id="extra-curricular" class="content-section active">
                <h2 class="section-heading">Extra Curricular Activities</h2>
                <div class="card card-content">
                    <ul class="list-none space-y-4 text-base">
                        <li>
                            <h3 class="text-accent text-lg">Outreach & Social Activities</h3>
                            <p>Active participation in various social and community service programs.</p>
                        </li>
                        <li>
                            <h3 class="text-accent text-lg">Student Mentoring & Advising</h3>
                            <p>Mentored B.Tech and M.Tech students for projects, career choices, and personal development.</p>
                        </li>
                        <li>
                            <h3 class="text-accent text-lg">Sports & Fitness</h3>
                            <p>Enthusiastic participant in college sports events and maintaining a regular fitness routine.</p>
                        </li>
                    </ul>
                </div>
            </section>

            <section id="gallery" class="content-section">
                <h2 class="section-heading">Gallery & Moments</h2>
                <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                    <div class="relative group">
                        <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/refs/heads/main/website%20phototes/gallery1.png" alt="Gallery Image 1" class="gallery-image">
                        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                            <p class="text-white text-sm">Conference Presentation</p>
                        </div>
                    </div>
                    <div class="relative group">
                        <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/refs/heads/main/website%20phototes/gallery2.png" alt="Gallery Image 2" class="gallery-image">
                        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                            <p class="text-white text-sm">Lab Work</p>
                        </div>
                    </div>
                    <div class="relative group">
                        <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/refs/heads/main/website%20phototes/gallery3.png" alt="Gallery Image 3" class="gallery-image">
                        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                            <p class="text-white text-sm">Graduation Day</p>
                        </div>
                    </div>
                    <div class="relative group">
                        <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/refs/heads/main/website%20phototes/gallery4.png" alt="Gallery Image 4" class="gallery-image">
                        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                            <p class="text-white text-sm">Family Time</p>
                        </div>
                    </div>
                </div>
            </section>

            <section id="contact" class="content-section">
                <h2 class="section-heading">Contact & Details</h2>
                <div class="card card-content">
                    <ul class="list-disc list-inside text-sm ml-4 space-y-2 mt-3">
                        <li><span class="font-semibold text-accent">Email:</span> <a href="mailto:yoursushmitha@example.com">yoursushmitha@example.com</a></li>
                        <li><span class="font-semibold text-accent">Phone:</span> +91-XXX-XXX-XXXX</li>
                        <li><span class="font-semibold text-accent">LinkedIn:</span> [Your LinkedIn Profile]</li>
                        <li><span class="font-semibold text-accent">Address:</span> Kavali, Nellore, Andhra Pradesh, India</li>
                    </ul>
                </div>
            </section>


        </div>
    </main>
    
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const navLinks = document.querySelectorAll('.nav-link');
            const contentSections = document.querySelectorAll('.content-section');

            const setActive = (targetId) => {
                // Deactivate all links and content
                navLinks.forEach(link => link.classList.remove('active'));
                contentSections.forEach(section => section.classList.remove('active'));

                // Activate the corresponding link and content
                const activeLink = document.querySelector(`.nav-link[data-target="${targetId}"]`);
                const activeSection = document.querySelector(`#${targetId}`);

                if (activeLink) activeLink.classList.add('active');
                if (activeSection) activeSection.classList.add('active');
            };

            // Event listener for navigation links
            navLinks.forEach(link => {
                link.addEventListener('click', (e) => {
                    e.preventDefault();
                    const targetId = link.getAttribute('data-target');
                    setActive(targetId);

                    // Update URL hash without jumping
                    history.pushState(null, '', `#${targetId}`);
                });
            });

            // Handle initial load based on URL hash
            const initialHash = window.location.hash.substring(1) || 'about';
            if (document.querySelector(`#${initialHash}`)) {
                setActive(initialHash);
            } else {
                setActive('about'); // Default to 'about' if hash is invalid
            }
        });
    </script>
</body>
</html>
