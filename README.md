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

        /* Card/Sub-Section Headings (H3) - REDUCED SIZE AND MARGINS HERE */
        h3 {
            color: #ffffff;
            font-size: 1.25rem; /* Reduced from 1.5rem (text-xl) */
            line-height: 1.75rem;
            font-weight: 600;
            margin-bottom: 0.25rem;
            margin-top: 0; /* Removing excess top gap */
            padding-top: 0;
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

        .container {
            max-width: 1400px;
        }
        
        /* ADJUSTED PROFILE PICTURE STYLES */
        .profile-picture {
            border-radius: 50%; /* Make it perfectly circular */
            border: 6px solid #fff;
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.2);
            /* Ensure the image fills the circle without distortion */
            width: 100%; /* Take full width of its parent div (e.g., w-36/w-48) */
            height: 100%; /* Take full height of its parent div */
            object-fit: cover; /* Crop to fit the circular shape */
        }
        /* Added to ensure the parent div of the profile picture is also a perfect square */
        .md\:w-1\/3 > .flex.justify-center {
            position: relative;
            width: 144px; /* Matches w-36, change to 192px for md:w-48 */
            height: 144px; /* Ensures a perfect square */
        }
        @media (min-width: 768px) { /* md breakpoint */
            .md\:w-1\/3 > .flex.justify-center {
                width: 192px; /* Matches md:w-48 */
                height: 192px; /* Ensures a perfect square */
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
                <a href="#extracurricular" class="nav-link" data-target="extracurricular">Awards and Recognition</a>
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
                        <li>Simulation of large-scale membrane reformers by a two-dimensional model. (FUSION-07), JNTU A.</li>
                        <li>Supercritical extraction. (TECHNOZION-07), NIT-W.</li>
                    </ul>
                </div>
            </section>

<section id="skills" class="content-section">
    <h2 class="section-heading">Skills & Core Expertise</h2>
    <div class="grid md:grid-cols-2 gap-4">

        <div class="card card-content md:col-span-2">
            <h3>Software & Simulation</h3>
            <p class="text-sm text-e0e0e0 italic mb-2">Advanced tools for Process Modeling, Simulation, and Data Analysis.</p>
            
            <h4 class="sub-sub-heading mt-2">Business Analytics Tools:</h4>
            <ul class="list-disc list-inside ml-4 space-y-1 text-sm">
                <li><span class="font-semibold">Power BI (Data visualization):</span> Used to visualize data and share insights across an organization. Connects to various data sources to create interactive dashboards and reports.</li>
                <li><span class="font-semibold">CRM software tool (Customer Relation Management).</span></li>
            </ul>

            <h4 class="sub-sub-heading mt-3">Statistical and Data Analysis Tools:</h4>
            <ul class="list-disc list-inside ml-4 space-y-1 text-sm">
                <li><span class="font-semibold">State ease:</span> Used for Econometrics, Panel Data, Epidemiology, and Social Science (for modeling the process and optimizing the model for best fit using regression).</li>
                <li><span class="font-semibold">Mini Tab:</span> Used for Quality Control, Six Sigma, and Basic Statistics Education.</li>
            </ul>
            
            <h4 class="sub-sub-heading mt-3">Process Simulation Tools (Macroscopic/Microscopic):</h4>
            <ul class="list-disc list-inside ml-4 space-y-1 text-sm">
                <li><span class="font-semibold">ASPEN Plus/HYSYS:</span> Expertise in modeling and simulation of steady-state and dynamic chemical processes (e.g., distillation, reactors, heat exchange).</li>
                <li><span class="font-semibold">ANSYS (Fluent, CFX):</span> Experienced in Computational Fluid Dynamics (CFD) for simulating fluid flow, heat transfer, and related phenomena.</li>
                <li><span class="font-semibold">AutoCAD:</span> Proficient in creating 2D/3D chemical process diagrams and equipment layouts.</li>
            </ul>

            <h4 class="sub-sub-heading mt-3">Other Technical Software:</h4>
            <ul class="list-disc list-inside ml-4 space-y-1 text-sm">
                <li><span class="font-semibold">Origin:</span> For high-quality graphing and data analysis.</li>
                <li><span class="font-semibold">Microsoft Office Suite:</span> Advanced proficiency (Word, Excel, PowerPoint).</li>
            </ul>
        </div>
        
        <div class="card card-content">
            <h3>Laboratory & Analytical Skills</h3>
            <p class="text-sm text-e0e0e0 italic mb-2">Hands-on experience with advanced materials synthesis and characterization.</p>
            <ul class="list-disc list-inside ml-4 space-y-2 text-sm">
                <li><span class="font-semibold">Chemical Synthesis:</span> Synthesis of Nano-materials (Lignin Nano capsules, Nano Cellulose), Hydrogel.</li>
                <li><span class="font-semibold">Electrochemical Testing:</span> Cyclic Voltammetry (CV), Galvanostatic Charge-Discharge (GCD), Electrochemical Impedance Spectroscopy (EIS).</li>
                <li><span class="font-semibold">Spectroscopy & Thermal Analysis:</span> FTIR, TGA, DSC, Raman Spectroscopy.</li>
                <li><span class="font-semibold">Microscopy & Diffraction:</span> SEM, TEM, AFM, XRD.</li>
                <li><span class="font-semibold">Process Equipment:</span> Batch/Semi-batch Reactors, High Pressure Autoclave, Ultrasonic Processors.</li>
            </ul>
        </div>

        <div class="card card-content">
            <h3>Teaching & Management Skills</h3>
            <p class="text-sm text-e0e0e0 italic mb-2">Academic and administrative competencies developed over years of teaching.</p>
            <ul class="list-disc list-inside ml-4 space-y-2 text-sm">
                <li><span class="font-semibold">Core Subjects:</span> Chemical Reaction Engineering, Transport Phenomena, Process Engineering Principles, Catalytic Engineering, Electrochemistry.</li>
                <li><span class="font-semibold">Management:</span> HR/Payroll Management, Placement Co-ordination, Curriculum Development, Team Leadership.</li>
                <li><span class="font-semibold">Mentoring:</span> Class Advisor/Mentor, Research Supervision for B.Tech/M.Tech students.</li>
            </ul>
        </div>
    </div>
</section>

<section id="extracurricular" class="content-section">
    <h2 class="section-heading">Awards & Professional Recognition</h2>
    <div class="card card-content">
        <ul class="list-disc list-inside text-sm ml-4 space-y-3 mt-3">
            <li class="flex justify-between items-start pr-4">
                <div class="flex-grow">
                    <span class="font-semibold text-accent block">Research Paper Recognition</span>
                    <span class="block italic text-xs">Ph.D. journal paper published in <span class="text-accent">Ultrasonics Sonochemistry</span> (IF: 9.336), a top-tier Elsevier journal.</span>
                </div>
            </li>
            <li class="flex justify-between items-start pr-4">
                <div class="flex-grow">
                    <span class="font-semibold text-accent block">Peer Reviewer Status (Elsevier Journals)</span>
                    <span class="block italic text-xs">Official reviewer for <span class="text-accent">Ultrasonics Sonochemistry (IF: 9.336)</span>, <span class="text-accent">Materials Letters (IF: 3.571)</span>, and <span class="text-accent">Journal of Materials Research and Technology (IF: 6.267)</span>.</span>
                </div>
                <a href="files/reviewer_certificates.png" target="_blank" class="text-xs bg-yellow-400 hover:bg-yellow-500 text-gray-900 font-bold py-1 px-2 rounded transition ml-4 flex-shrink-0 mt-1">View Certificates</a>
            </li>
            <li class="flex justify-between items-start pr-4">
                <div class="flex-grow">
                    <span class="font-semibold text-accent block">Fellowships & Scholarships</span>
                    <span class="block italic text-xs">Awarded the <span class="text-accent">MHRD Scholarship</span> during Ph.D. and <span class="text-accent">AICTE Fellowship</span> during M.Tech.</span>
                </div>
            </li>
            <li class="flex justify-between items-start pr-4">
                <div class="flex-grow">
                    <span class="font-semibold text-accent block">Professional Memberships</span>
                    <span class="block italic text-xs">Associate Member of the <span class="text-accent">Indian Institute of Chemical Engineers (IICHE)</span> and the <span class="text-accent">Institution of Engineers (India) [IEI]</span>.</span>
                </div>
            </li>
        </ul>
    </div>
</section>

<section id="extra-curricular" class="content-section">
   <section id="extra-curricular" class="content-section">
    <h2 class="section-heading">Extra Curricular Activities & Interests</h2>
    <div class="card card-content">
        <ul class="list-disc list-inside text-sm ml-4 space-y-3 mt-3">
            <li>
                <span class="font-semibold text-accent inline">Literary and Creative Writing:</span>
                Contributed articles to college magazines and online platforms focused on science communication and technology ethics.
            </li>
            <li>
                <span class="font-semibold text-accent inline">Community Engagement:</span>
                Involved in organizing student mentorship programs and career counseling sessions for underprivileged students.
            </li>
            <li>
                <span class="font-semibold text-accent inline">Technical Events:</span>
                Served as Event Coordinator for national-level technical symposiums, managing logistics for up to 500 participants.
            </li>
             <li>
                <span class="font-semibold text-accent inline">Trekking and Nature Exploration:</span>
                Regular participation in local and regional treks, fostering teamwork and resilience.
            </li>
        </ul>
    </div>
</section>

<section id="gallery" class="content-section">
    <h2 class="section-heading">Gallery: Research, Work & Education</h2>
    <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
        <div class="relative group">
            <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/main/website%20phototes/research1.png" alt="Lab Research Work" class="gallery-image">
            <div class="absolute inset-0 bg-gray-900 bg-opacity-70 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                <p class="text-white text-xs text-center p-2 font-semibold">Nanoparticle Synthesis</p>
            </div>
        </div>
        <div class="relative group">
            <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/main/website%20phototes/conference1.png" alt="Conference Presentation" class="gallery-image">
            <div class="absolute inset-0 bg-gray-900 bg-opacity-70 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                <p class="text-white text-xs text-center p-2 font-semibold">International Conference</p>
            </div>
        </div>
        <div class="relative group">
            <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/main/website%20phototes/teaching1.png" alt="Teaching Moment" class="gallery-image">
            <div class="absolute inset-0 bg-gray-900 bg-opacity-70 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                <p class="text-white text-xs text-center p-2 font-semibold">Guest Lecture at JNTU</p>
            </div>
        </div>
        <div class="relative group">
            <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/main/website%20phototes/phd_grad.png" alt="PhD Graduation Ceremony" class="gallery-image">
            <div class="absolute inset-0 bg-gray-900 bg-opacity-70 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                <p class="text-white text-xs text-center p-2 font-semibold">PhD Graduation (NITW)</p>
            </div>
        </div>
        <div class="relative group">
            <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/main/website%20phototes/vizag_steel.png" alt="Vizag Steel Plant" class="gallery-image">
            <div class="absolute inset-0 bg-gray-900 bg-opacity-70 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                <p class="text-white text-xs text-center p-2 font-semibold">Industrial Training (VSP)</p>
            </div>
        </div>
        <div class="relative group">
            <img src="https://raw.githubusercontent.com/sushmitha-d-nitw/Dr.D.SUSHMITHA/main/website%20phototes/book_chapter.png" alt="Book Chapter Cover" class="gallery-image">
            <div class="absolute inset-0 bg-gray-900 bg-opacity-70 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                <p class="text-white text-xs text-center p-2 font-semibold">Book Chapter Contribution</p>
            </div>
        </div>
    </div>
</section>

<section id="contact" class="content-section">
    <h2 class="section-heading">Contact & Professional Links</h2>
    <div class="card card-content">
        <div class="grid md:grid-cols-2 gap-4">
            <div>
                <h3>Personal Contact</h3>
                <ul class="list-disc list-inside text-sm ml-4 space-y-2 mt-2">
                    <li><span class="font-semibold text-accent">Email:</span> <a href="mailto:sushmithache@gmail.com">sushmithache@gmail.com</a></li>
                    <li><span class="font-semibold text-accent">Mobile:</span> +91 94901XXXXX (Available upon request)</li>
                    <li><span class="font-semibold text-accent">Location:</span> Hyderabad, Telangana, India</li>
                </ul>
            </div>
            <div>
                <h3>Professional Profiles</h3>
                <ul class="list-disc list-inside text-sm ml-4 space-y-2 mt-2">
                    <li><span class="font-semibold text-accent">LinkedIn:</span> <a href="https://www.linkedin.com/in/sushmitha-d-ph-d-35431526" target="_blank">Dr. D. Sushmitha, Ph.D.</a></li>
                    <li><span class="font-semibold text-accent">Google Scholar:</span> <a href="https://scholar.google.com/citations?user=L07p48gAAAAJ" target="_blank">View Citations</a></li>
                    <li><span class="font-semibold text-accent">ORCID:</span> <a href="https://orcid.org/0000-0002-9844-4866" target="_blank">0000-0002-9844-4866</a></li>
                    <li><span class="font-semibold text-accent">ResearchGate:</span> <a href="https://www.researchgate.net/profile/D-Sushmitha" target="_blank">Dr. D. Sushmitha</a></li>
                </ul>
            </div>
        </div>
        <h3 class="mt-6">Reference</h3>
        <p class="text-sm italic mt-2">Professional references and letter of recommendation are available upon request.</p>
    </div>
</section>
        </div> 
    </main>

    <footer class="text-center py-3 text-xs border-t border-gray-700 mt-4">
        <p class="text-gray-300">&copy; <span id="current-year"></span> Dr. D. Sushmitha. All rights reserved.</p>
        <p class="text-gray-400">Chemical Engineering Specialist | Built with Tailwind CSS and Vanilla JS.</p>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Set current year in footer
            document.getElementById('current-year').textContent = new Date().getFullYear();

            const navLinks = document.querySelectorAll('.nav-link');
            const sections = document.querySelectorAll('.content-section');

            // Function to handle section display
            function showSection(targetId) {
                // Deactivate all links and sections
                navLinks.forEach(link => link.classList.remove('active'));
                sections.forEach(section => section.classList.remove('active'));

                // Activate the target link and section
                const targetLink = document.querySelector(`.nav-link[data-target="${targetId}"]`);
                const targetSection = document.getElementById(targetId);

                if (targetLink) {
                    targetLink.classList.add('active');
                }
                if (targetSection) {
                    targetSection.classList.add('active');
                    targetSection.scrollTop = 0; // Scroll to top of the new section
                }
            }

            // Event listener for navigation links
            navLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    // Prevent default anchor link behavior (which causes full page scroll)
                    e.preventDefault(); 
                    
                    const targetId = this.getAttribute('data-target');
                    
                    // Update the URL hash (optional, but good for back/forward buttons)
                    history.pushState(null, '', `#${targetId}`);

                    showSection(targetId);
                });
            });

            // Handle initial load based on URL hash (e.g., if page is loaded with #experience)
            function handleHashChange() {
                const hash = window.location.hash.substring(1); // Get hash without '#'
                const initialTargetId = hash || 'about'; // Default to 'about' if no hash

                // Use a slight delay to ensure the fadeIn animation runs correctly on load
                setTimeout(() => {
                    showSection(initialTargetId);
                }, 10);
            }
            
            // Run on load
            handleHashChange();

            // Also listen for hash changes (back/forward button)
            window.addEventListener('hashchange', handleHashChange);
        });
    </script>
</body>
</html>
