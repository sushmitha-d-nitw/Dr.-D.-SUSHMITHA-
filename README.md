<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dr. D. Sushmitha | Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Chosen Palette: Striking Blue & Gold -->
    <!-- Application Structure Plan: The application is designed as a single-page portfolio with a fixed navigation header. The core interaction is a "tabbed" content view: clicking a navigation link hides all other sections and displays only the relevant one. This structure was chosen to directly fulfill the user's request for focused content presentation, preventing distractions and long scrolling. The user flow is simple: Land on Home -> Click Nav Item -> View Focused Section -> Click Another Nav Item. This is more direct than a long-scroll page for a user who wants to see specific information quickly. -->
    <!-- Visualization & Content Choices: The portfolio uses structured text sections (cards, lists, timelines) to present resume information clearly. Goal: Inform -> Method: Card-based layouts for experience/education and structured lists for publications/skills. Interaction: The primary interaction is the navigation system that reveals content sections. This avoids overwhelming the user with all information at once. Publication titles are hyperlinked as requested, enhancing usability for academic visitors. No complex data visualizations were needed for this text-based resume content. -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #F8F9FA;
            color: #333333;
        }
        h1, h2, h3 {
            font-family: 'Playfair Display', serif;
        }
        .nav-link {
            position: relative;
            transition: color 0.3s ease;
        }
        .nav-link.active {
            color: #0052A5;
        }
        .nav-link.active::after, .nav-link:hover::after {
            content: '';
            position: absolute;
            bottom: -4px;
            left: 0;
            width: 100%;
            height: 2px;
            background-color: #F5A623;
        }
        .content-section {
            display: none;
            animation: fadeIn 0.8s;
        }
        .content-section.visible {
            display: block;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .timeline::before {
            content: '';
            position: absolute;
            left: 10px;
            top: 0;
            bottom: 0;
            width: 2px;
            background-color: #e2e8f0;
        }
        .timeline-item::before {
            content: '';
            position: absolute;
            left: -19px;
            top: 6px;
            width: 14px;
            height: 14px;
            border-radius: 50%;
            background-color: #F5A623;
            border: 2px solid #F8F9FA;
        }
    </style>
</head>
<body class="antialiased">

    <header class="bg-white/80 backdrop-blur-md shadow-sm sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <h1 class="text-2xl font-bold text-[#0052A5]">Dr. D. Sushmitha</h1>
            <div class="hidden md:flex space-x-8">
                <a href="#home" class="nav-link active">Home</a>
                <a href="#about" class="nav-link">About</a>
                <a href="#experience" class="nav-link">Experience</a>
                <a href="#education" class="nav-link">Education</a>
                <a href="#publications" class="nav-link">Publications</a>
                <a href="#awards" class="nav-link">Awards</a>
                <a href="#skills" class="nav-link">Skills</a>
                <a href="#extracurricular" class="nav-link">Extracurriculars</a>
                <a href="#contact" class="nav-link">Contact</a>
            </div>
            <button id="mobile-menu-button" class="md:hidden text-2xl">☰</button>
        </nav>
        <div id="mobile-menu" class="hidden md:hidden bg-white px-6 pb-4">
            <a href="#home" class="block py-2 nav-link-mobile">Home</a>
            <a href="#about" class="block py-2 nav-link-mobile">About</a>
            <a href="#experience" class="block py-2 nav-link-mobile">Experience</a>
            <a href="#education" class="block py-2 nav-link-mobile">Education</a>
            <a href="#publications" class="block py-2 nav-link-mobile">Publications</a>
            <a href="#awards" class="block py-2 nav-link-mobile">Awards</a>
            <a href="#skills" class="block py-2 nav-link-mobile">Skills</a>
            <a href="#extracurricular" class="block py-2 nav-link-mobile">Extracurriculars</a>
            <a href="#contact" class="block py-2 nav-link-mobile">Contact</a>
        </div>
    </header>

    <main class="container mx-auto p-6 md:p-8">
        
        <section id="home" class="content-section visible min-h-[70vh] flex items-center">
            <div class="text-center w-full">
                <h2 class="text-5xl md:text-7xl font-bold text-[#0052A5]">Dr. D. Sushmitha</h2>
                <p class="text-xl md:text-2xl mt-4 text-gray-600">Academician, Researcher, and Chemical Engineer</p>
                <p class="max-w-3xl mx-auto mt-6 text-gray-500">
                    A dedicated and results-oriented professional with over 10 years of diverse expertise in academia and industry, specializing in Chemical Engineering, Biotechnology, and Sustainable Processes. Passionate about teaching, research, and fostering innovation.
                </p>
                <a href="#contact" class="inline-block bg-[#0052A5] text-white font-bold py-3 px-8 rounded-full mt-8 hover:bg-[#00387a] transition-colors duration-300">Get In Touch</a>
            </div>
        </section>

        <section id="about" class="content-section">
            <h2 class="text-4xl font-bold mb-6 text-[#0052A5]">About Me</h2>
            <div class="bg-white p-8 rounded-lg shadow-md space-y-4 text-lg text-gray-700 leading-relaxed">
                <p>
                    I am an accomplished academician and researcher with a Ph.D. in Chemical Engineering from NIT Warangal. My career spans over a decade, encompassing roles as an Assistant Professor, Researcher, Guest Faculty, and Business Development Manager. This diverse background has equipped me with a robust skill set in teaching, curriculum development, and student mentorship.
                </p>
                <p>
                    My primary research interest lies in the domain of <strong class="text-[#0052A5]">biodiesel production from non-edible oils</strong>, focusing on process optimization, kinetic modeling, and the application of heterogeneous catalysts. I am deeply committed to exploring sustainable energy solutions and contributing to the field through rigorous research and impactful publications.
                </p>
                <p>
                    Throughout my academic journey, I have undertaken numerous responsibilities beyond teaching, including serving as a Placement Coordinator, Class Advisor, and Hostel Warden, reflecting my dedication to holistic student development. I thrive in dynamic environments where I can leverage my expertise to educate the next generation of engineers and scientists.
                </p>
            </div>
        </section>

        <section id="experience" class="content-section">
             <h2 class="text-4xl font-bold mb-8 text-[#0052A5]">Professional Experience</h2>
             <div class="space-y-8">
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex justify-between items-start">
                        <div>
                            <h3 class="text-2xl font-bold text-[#0052A5]">Assistant Professor (Temporary)</h3>
                            <p class="text-lg font-medium text-gray-700">Department of Biotechnology, IST JNTU-H, Kukatpally</p>
                        </div>
                        <span class="text-md font-semibold text-gray-500">Jan 2025 - Present</span>
                    </div>
                    <div class="mt-4 text-gray-600">
                        <p><strong>Subjects Taught:</strong> Process Engineering Principles (B.Tech 2nd year, M.Sc 2nd year)</p>
                        <p><strong>Labs Conducgted:</strong> Chemical Reaction Engineering Lab, Enzyme Engineering Lab</p>
                    </div>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md">
                     <div class="flex justify-between items-start">
                        <div>
                            <h3 class="text-2xl font-bold text-[#0052A5]">Assistant Professor</h3>
                            <p class="text-lg font-medium text-gray-700">Department of Petrochemical Technology, Excel Engineering College, Tamil Nadu</p>
                        </div>
                        <span class="text-md font-semibold text-gray-500">May 2022 - Nov 2022</span>
                    </div>
                    <div class="mt-4 text-gray-600">
                        <p><strong>Courses Taught:</strong> Electrochemical Process Technology, Chemical Reaction Engineering-I & II, Catalytic reaction engineering, Fluid Mechanics.</p>
                        <p><strong>Academic Responsibilities:</strong> Placement Co-ordinator; Class Advisor/Mentor; Class committee Co-ordinator; Hostel Warden; Internship Co-ordinator.</p>
                    </div>
                </div>
                 <div class="bg-white p-6 rounded-lg shadow-md">
                     <div class="flex justify-between items-start">
                        <div>
                            <h3 class="text-2xl font-bold text-[#0052A5]">Business Development Manager & Sales Manager</h3>
                            <p class="text-lg font-medium text-gray-700">Riss InfoTech</p>
                        </div>
                        <span class="text-md font-semibold text-gray-500">Nov 2020 - Jan 2021</span>
                    </div>
                    <ul class="list-disc list-inside mt-4 text-gray-600 space-y-2">
                        <li>Responsible for business development and sales activities.</li>
                        <li>Engaged in market analysis and client relationship management.</li>
                    </ul>
                </div>
                 <div class="bg-white p-6 rounded-lg shadow-md">
                     <div class="flex justify-between items-start">
                        <div>
                            <h3 class="text-2xl font-bold text-[#0052A5]">Guest Faculty</h3>
                            <p class="text-lg font-medium text-gray-700">Department of Petrochemical Engineering, JNTU-H, Kukatpally</p>
                        </div>
                        <span class="text-md font-semibold text-gray-500">Jan 2017 - Aug 2017</span>
                    </div>
                    <div class="mt-4 text-gray-600">
                        <p><strong>Courses Taught:</strong> Process Dynamics and Control, Chemical Reaction Engineering, Process Instrumentation.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="education" class="content-section">
            <h2 class="text-4xl font-bold mb-8 text-[#0052A5]">Education</h2>
            <div class="space-y-8">
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex justify-between items-start">
                        <div>
                            <h3 class="text-2xl font-bold text-[#0052A5]">Ph.D. in Chemical Engineering</h3>
                            <p class="text-lg font-medium text-gray-700">National Institute of Technology, Warangal (NITW)</p>
                        </div>
                        <span class="text-md font-semibold text-gray-500">2012 - 2017</span>
                    </div>
                </div>
                 <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex justify-between items-start">
                        <div>
                            <h3 class="text-2xl font-bold text-[#0052A5]">Master of Technology (M.Tech)</h3>
                            <p class="text-lg font-medium text-gray-700">Jawaharlal Nehru Technological University, Anantapur (JNTUA)</p>
                        </div>
                        <span class="text-md font-semibold text-gray-500">2007 - 2009</span>
                    </div>
                    <p class="mt-2 text-gray-600">Specialization: Biotechnology</p>
                </div>
                 <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex justify-between items-start">
                        <div>
                            <h3 class="text-2xl font-bold text-[#0052A5]">Bachelor of Technology (B.Tech)</h3>
                            <p class="text-lg font-medium text-gray-700">Jawaharlal Nehru Technological University, Anantapur (JNTUA)</p>
                        </div>
                        <span class="text-md font-semibold text-gray-500">2003 - 2007</span>
                    </div>
                    <p class="mt-2 text-gray-600">Specialization: Chemical Engineering</p>
                </div>
            </div>
        </section>

        <section id="publications" class="content-section">
            <h2 class="text-4xl font-bold mb-8 text-[#0052A5]">Research Publications</h2>
            <div class="space-y-8">
                <div>
                    <h3 class="text-2xl font-bold text-[#0052A5] mb-4">Journals</h3>
                    <ul class="list-none space-y-4 text-gray-700">
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="https://www.sciencedirect.com/science/article/pii/S221499371730079X" target="_blank" class="text-lg font-semibold text-[#0052A5] hover:underline">Kinetic study of biodiesel production from unrefined Nahar oil (Mesua ferrea L) using calcium diglycolate as heterogeneous nanocatalyst</a>
                            <p class="text-gray-600 mt-1"><strong>Journal:</strong> Journal of the Taiwan Institute of Chemical Engineers</p>
                            <p class="text-gray-600"><strong>Impact Factor:</strong> 4.794</p>
                            <p class="text-gray-600"><strong>Pages:</strong> 155-163</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="https://onlinelibrary.wiley.com/doi/full/10.1002/cjce.22744" target="_blank" class="text-lg font-semibold text-[#0052A5] hover:underline">Green Synthesis of Zinc Oxide Nanoparticles with Mesua Ferrea Seed Oil as Reducing Agent and Evaluation of Its Catalytic Activity for Biodiesel Production</a>
                            <p class="text-gray-600 mt-1"><strong>Journal:</strong> The Canadian Journal of Chemical Engineering</p>
                            <p class="text-gray-600"><strong>Impact Factor:</strong> 2.009</p>
                            <p class="text-gray-600"><strong>Pages:</strong> 163-172</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="https://www.researchgate.net/publication/318712368_Process_optimization_of_biodiesel_production_from_Mesua_ferrea_L_seed_oil_with_calcium_diglycolate_as_a_heterogeneous_nanocatalyst" target="_blank" class="text-lg font-semibold text-[#0052A5] hover:underline">Process optimization of biodiesel production from Mesua ferrea L seed oil with calcium diglycolate as a heterogeneous nanocatalyst</a>
                            <p class="text-gray-600 mt-1"><strong>Journal:</strong> Particulate Science and Technology</p>
                            <p class="text-600"><strong>Impact Factor:</strong> 1.5</p>
                            <p class="text-gray-600"><strong>Pages:</strong> 1-7</p>
                        </li>
                    </ul>
                </div>

                <div>
                    <h3 class="text-2xl font-bold text-[#0052A5] mb-4">Book & Book Chapters</h3>
                    <ul class="list-none space-y-4 text-gray-700">
                         <li class="bg-white p-6 rounded-lg shadow-md">
                            <p class="text-lg font-semibold">
                                <a href="https://link.springer.com/chapter/10.1007/978-981-15-4680-4_4" target="_blank" class="text-[#0052A5] hover:underline">
                                    Valorization of Waste Cooking Oil to Biodiesel Using Waste Eggshell-Derived Catalysts
                                </a>
                                <br>
                                <strong>Book:</strong> <span class="font-normal">Advanced Chemical Engineering</span>
                            </p>
                             <p class="text-gray-600 mt-1">
                                 <strong>Publisher:</strong> <span class="font-normal">Springer Singapore</span>
                             </p>
                            <p class="text-gray-600 mt-1">
                                 <strong>ISBN:</strong> <span class="font-normal">978-981-15-4680-4</span>
                             </p>
                             <p class="text-gray-600">
                                 <strong>Pages:</strong> <span class="font-normal">153-177</span>
                             </p>
                         </li>
                    </ul>
                </div>
            
                <div>
                    <h3 class="text-2xl font-bold text-[#0052A5] mb-4">International Conferences</h3>
                    <ul class="list-none space-y-4 text-gray-700">
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="https://ieeexplore.ieee.org/document/9082710" target="_blank" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                1. Study on Biodiesel Production from Unrefined Nahar (Mesua Ferrea L) Oil Using Calcium Diglycolate Heterogeneous Catalyst: International Conference on New Frontiers in Engineering, Science and Technology, NIT-Warangal.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICNFEST, NIT-Warangal</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> 978-1-7281-2294-8</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                2. Synthesis of Green Nanoparticles from Agro-waste Materials Using Bio-molecules, International Conference on Advanced Functional Materials, University of Kerala, Trivandrum.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICAFM, University of Kerala, Trivandrum</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                         <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                3. A Critical Review on Nano Catalyst for Biofuel Production from Algal Biomass, International Conference on Biotechnology and Bioengineering, CBIT, Gandipet, Hyderabad.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICBB, CBIT, Gandipet</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                4. A Green Synthesis of Nano Bio-Catalyst from Natural Waste Material: International Conference on Science, Technology, and Management, University of Hyderabad.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICSTM, University of Hyderabad</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                         <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                5. Design of Lab Scale Bio-Reactor for Biodiesel Production: International Conference on Nanotechnology, JNTU-H, Kukatpally, Hyderabad.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICN, JNTU-H, Kukatpally</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                         <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                6. Synthesis of Bio-Lubricants from Mahua Oil Using Nano Catalyst: International Conference on Renewable Energy and Sustainable Environment, MGR University, Chennai.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICRESE, MGR University, Chennai</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                7. Bioconversion of Non-Edible Oil to Biofuel: International Conference on Biofuel and Bio-Economy, VIT University, Vellore.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICBB, VIT University, Vellore</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                8. Catalytic Transesterification of Pongamia Pinnata Oil Using Nano Catalyst: International Conference on Chemical, Civil and Mechanical Engineering, VITS, Guntur.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICCME, VITS, Guntur</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                9. Bio-oil Production from Algal Biomass: International Conference on Algae as Sustainable Energy Source, JNTU-H, Kukatpally, Hyderabad.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICAAS, JNTU-H, Kukatpally</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                10. A Review on Bio-refinery for Sustainable Biofuel Production: International Conference on Green Technology for Sustainable Environment, JNTU-H, Kukatpally, Hyderabad.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICGTSE, JNTU-H, Kukatpally</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                11. Biogas Production from Waste Biomass: International Conference on Biotechnology, Bioengineering and Biomaterials, BITS, Hyderabad.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICBBB, BITS, Hyderabad</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                12. Recent Trends in Bioremediation: International Conference on Environmental Science and Technology, IIT, Hyderabad.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICSET, IIT, Hyderabad</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <a href="#" class="text-lg font-semibold text-[#0052A5] hover:underline">
                                13. Bio-hydrogen Production from Fermentative Pathway: International Conference on Advanced Materials and Technology, NIT-Warangal.
                            </a>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> ICAMT, NIT-Warangal</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                    </ul>
                </div>

                <div>
                    <h3 class="text-2xl font-bold text-[#0052A5] mb-4">National Conferences</h3>
                    <ul class="list-none space-y-4 text-gray-700">
                        <li class="bg-white p-6 rounded-lg shadow-md">
                            <p class="text-lg font-semibold">
                                1. Review of Green Energy Resources: National Conference on Recent Advances in Chemical Engineering, NIT-Warangal.
                            </p>
                            <p class="text-gray-600 mt-1"><strong>Conference Name:</strong> RACE, NIT-Warangal</p>
                            <p class="text-gray-600"><strong>ISBN:</strong> Not Provided</p>
                        </li>
                    </ul>
                </div>

            </div>
        </section>

        <section id="awards" class="content-section">
             <h2 class="text-4xl font-bold mb-8 text-[#0052A5]">Awards & Recognitions</h2>
             <div class="space-y-6 text-gray-700">
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <p class="text-lg font-medium">Recipient of the <span class="text-[#F5A623] font-semibold">Best Paper Award</span> at the National Conference "Research Conclave-17," held at the National Institute of Technology Warangal, for outstanding research contributions.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <p class="text-lg font-medium">Officially recognized as a <span class="text-[#F5A623] font-semibold">reviewer for three high-impact Elsevier journals</span> ("Renewable Energy," "Materials Today Proceedings," and "Journal of King Saud University - Engineering Science") due to a high degree of domain expertise and professional excellence.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <p class="text-lg font-medium"><span class="text-[#F5A623] font-semibold">Successfully qualified for the All India GATE exam three times</span>, demonstrating a consistent and profound understanding of core engineering principles.</p>
                </div>
                 <div class="bg-white p-6 rounded-lg shadow-md">
                    <p class="text-lg font-medium">Awarded a prestigious <span class="text-[#F5A623] font-semibold">scholarship from the Ministry of Human Resources Development (MHRD)</span>, Government of India, to support doctoral studies in Chemical Engineering, validating the merit of my academic pursuits.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <p class="text-lg font-medium">Received the <span class="text-[#F5A623] font-semibold">All India Council for Technical Education (AICTE) fellowship</span> during my M.Tech at NIT-W, a testament to my academic distinction.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <p class="text-lg font-medium">An <span class="text-[#F5A623] font-semibold">Associate Member of the Indian Institute of Chemical Engineers (IICHE)</span> since December 2017, reflecting my commitment to the professional community.</p>
                </div>
                 <div class="bg-white p-6 rounded-lg shadow-md">
                    <p class="text-lg font-medium">An <span class="text-[#F5A623] font-semibold">Associate Member of the Institute of Engineers India (IEI)</span> since April 2023, showcasing ongoing professional engagement.</p>
                </div>
            </div>
        </section>
        
        <section id="skills" class="content-section">
            <h2 class="text-4xl font-bold mb-8 text-[#0052A5]">Skills</h2>
            <div class="space-y-6">
                <div>
                    <h3 class="text-2xl font-bold mb-4 text-[#0052A5]">General Software & Technical Skills</h3>
                     <ul class="list-none space-y-2 text-gray-700">
                        <li class="bg-white p-4 rounded-lg shadow-md">Aspen Hysys</li>
                        <li class="bg-white p-4 rounded-lg shadow-md">Ansys</li>
                        <li class="bg-white p-4 rounded-lg shadow-md">SolidWorks</li>
                        <li class="bg-white p-4 rounded-lg shadow-md">CAD</li>
                        <li class="bg-white p-4 rounded-lg shadow-md">Microsoft Office, Excel, and Free AI tools for academics</li>
                    </ul>
                </div>
                <div>
                    <h3 class="text-2xl font-bold mb-4 text-[#0052A5]">🔬 Analytical Instrumentation & Laboratory Techniques</h3>
                    <ul class="list-none space-y-2 text-gray-700">
                        <li class="bg-white p-4 rounded-lg shadow-md">
                            <strong>Spectroscopic Techniques (FTIR, NMR, Raman):</strong> Functional group identification, molecular structure elucidation, and vibrational analysis.
                        </li>
                        <li class="bg-white p-4 rounded-lg shadow-md">
                            <strong>Chromatographic Techniques (HPLC, GPC):</strong> Compound separation and quantification, and molecular size-based separation for polymer analysis.
                        </li>
                        <li class="bg-white p-4 rounded-lg shadow-md">
                            <strong>Thermal Analysis (TGA, DTA):</strong> Mass change monitoring with temperature and heat flow comparison.
                        </li>
                        <li class="bg-white p-4 rounded-lg shadow-md">
                            <strong>Particle & Sample Handling (PSA, Centrifuge):</strong> Granulometric profiling of powders and suspensions, and phase separation and sample preparation.
                        </li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="extracurricular" class="content-section">
            <h2 class="text-4xl font-bold mb-8 text-[#0052A5]">Extracurricular Activities</h2>
            <div class="relative pl-8 timeline">
                <div class="timeline-item relative pb-8">
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <p class="font-semibold text-lg text-gray-700">Won first prize in a Running Race at JNTU-College Anantapur during 2k7.</p>
                        <p class="text-sm text-gray-500 mt-1">2007</p>
                    </div>
                </div>
                 <div class="timeline-item relative pb-8">
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <p class="font-semibold text-lg text-gray-700">Won first prize in Kho-kho at JNTU-Engineering College Anantapur in 2k7.</p>
                    </div>
                </div>
                 <div class="timeline-item relative pb-8">
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <p class="font-semibold text-lg text-gray-700">Actively participated in cultural festival events "FUSION-05" and "SCHEMCON-06", an Inter National level Symposium at JNTU, Engineering College Anantapur.</p>
                    </div>
                </div>
                 <div class="timeline-item relative pb-8">
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <p class="font-semibold text-lg text-gray-700">Bagged National level certificate for Participated in "All India Inter school cultural festival" at Bangalore in 2k, 2k1, during ninth and tenth class.</p>
                    </div>
                </div>
                 <div class="timeline-item relative pb-8">
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <p class="font-semibold text-lg text-gray-700">Certified and badged for Collecting money to "Help age India" In third class.</p>
                    </div>
                </div>
            </div>
        </section>
        
        <section id="contact" class="content-section">
            <h2 class="text-4xl font-bold mb-8 text-[#0052A5]">Contact</h2>
            <div class="bg-white p-8 rounded-lg shadow-md max-w-2xl mx-auto text-lg text-gray-700">
                <p class="mb-4">Feel free to reach out to me for academic collaborations, research inquiries, or professional opportunities.</p>
                <div class="space-y-4">
                    <div class="flex items-center space-x-4">
                        <span class="text-[#F5A623] text-2xl">✉️</span>
                        <a href="mailto:sushmitha.d.nitw@gmail.com" class="hover:underline">sushmitha.d.nitw@gmail.com</a>
                    </div>
                    <div class="flex items-center space-x-4">
                        <span class="text-[#F5A623] text-2xl">📞</span>
                        <span>+91 7981541047</span>
                    </div>
                    <div class="flex items-center space-x-4">
                        <span class="text-[#F5A623] text-2xl">🌐</span>
                        <a href="https://www.linkedin.com/in/sushmitha-d-ph-d-752187a5" target="_blank" class="hover:underline">LinkedIn Profile</a>
                    </div>
                    <div class="flex items-center space-x-4">
                        <span class="text-[#F5A623] text-2xl">📍</span>
                        <span>Hyderabad, Telangana, India</span>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const navLinks = document.querySelectorAll('.nav-link, .nav-link-mobile');
            const sections = document.querySelectorAll('.content-section');
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');

            const showSection = (id) => {
                sections.forEach(section => {
                    section.classList.remove('visible');
                });
                document.getElementById(id).classList.add('visible');
            };

            const setActiveLink = (id) => {
                navLinks.forEach(link => {
                    link.classList.remove('active');
                });
                document.querySelector(`a[href="#${id}"]`).classList.add('active');
            };

            navLinks.forEach(link => {
                link.addEventListener('click', (e) => {
                    const sectionId = link.getAttribute('href').substring(1);
                    showSection(sectionId);
                    setActiveLink(sectionId);
                    if (mobileMenu.classList.contains('flex')) {
                        mobileMenu.classList.remove('flex');
                        mobileMenu.classList.add('hidden');
                    }
                });
            });

            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
                mobileMenu.classList.toggle('flex');
                mobileMenu.classList.toggle('flex-col');
            });
            
            // Initial view
            showSection('home');
        });
    </script>
</body>
</html>
