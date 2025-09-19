# Professional-portfolio-
My professional portfolio website
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dr. D. Sushmitha - Personal Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f3f4f6;
            color: #374151;
        }
        .container {
            max-width: 1200px;
        }
        .section-heading {
            border-bottom: 2px solid #e5e7eb;
            padding-bottom: 0.5rem;
            margin-bottom: 1.5rem;
        }
        .card {
            background-color: #ffffff;
            border-radius: 0.75rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
            transition: transform 0.3s ease-in-out;
        }
        .card:hover {
            transform: translateY(-5px);
        }
        .list-disc-outside {
            list-style-type: disc;
            list-style-position: outside;
            padding-left: 1.5rem;
        }
        .no-link-color {
            color: inherit;
            text-decoration: none;
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-700">

    <!-- Header Section -->
    <header class="bg-white shadow-sm py-8 md:py-12">
        <div class="container mx-auto px-4 text-center">
            <h1 class="text-4xl md:text-5xl font-extrabold text-gray-900 mb-2">Dr. D. Sushmitha</h1>
            <p class="text-lg md:text-xl text-gray-600 font-medium">Assistant Professor, Researcher & Manager</p>
            <div class="flex flex-col md:flex-row justify-center items-center mt-4 space-y-2 md:space-y-0 md:space-x-4 text-sm md:text-base">
                <a href="tel:7981541047" class="flex items-center text-blue-600 hover:text-blue-800 transition-colors duration-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-1" viewBox="0 0 20 20" fill="currentColor"><path d="M2 3a1 1 0 011-1h2.153a1 1 0 01.986.836l.74 4.435a1 1 0 01-.54 1.06l-1.548.774a11.037 11.037 0 006.101 6.101l.774-1.548a1 1 0 011.06-.54l4.435.74a1 1 0 01.836.986V17a1 1 0 01-1 1h-2C7.373 18 3 13.627 3 8V5a1 1 0 011-1z"/></svg>
                    7981541047
                </a>
                <a href="mailto:sushmitha.d.nitw@gmail.com" class="flex items-center text-blue-600 hover:text-blue-800 transition-colors duration-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-1" viewBox="0 0 20 20" fill="currentColor"><path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z"/><path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z"/></svg>
                    sushmitha.d.nitw@gmail.com
                </a>
                <a href="https://scholar.google.com/citations?user=Qk1uTQYAAAAJ" target="_blank" class="flex items-center text-blue-600 hover:text-blue-800 transition-colors duration-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-1" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2c5.523 0 10 4.477 10 10s-4.477 10-10 10S2 17.523 2 12 6.477 2 12 2zm-1 15h2V7h-2v10zM12 6a1 1 0 100-2 1 1 0 000 2z"/></svg>
                    Google Scholar
                </a>
                <a href="https://orcid.org/0000-0002-1125-6904" target="_blank" class="flex items-center text-blue-600 hover:text-blue-800 transition-colors duration-300">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-1" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2c5.523 0 10 4.477 10 10s-4.477 10-10 10S2 17.523 2 12 6.477 2 12 2zm-1 15h2V7h-2v10zM12 6a1 1 0 100-2 1 1 0 000 2z"/></svg>
                    ORCID
                </a>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="container mx-auto px-4 py-8 md:py-12 space-y-12">
        
        <!-- About Section -->
        <section id="about" class="card p-6 md:p-8">
            <h2 class="text-2xl md:text-3xl font-bold text-gray-800 mb-4 section-heading">About</h2>
            <p class="text-base md:text-lg leading-relaxed">
                With over 9 years and 7 months of diverse expertise, Dr. D. Sushmitha is a dedicated academician and researcher specializing in Chemical Engineering. Her background includes 3 years and 5 months as an Assistant Professor, 6 years as a Researcher, and 2 months as a Manager. Her work focuses on areas such as process intensification, biorefinery, polymer chemistry, and new energy and renewables. She is currently working as an Assistant Professor (temporary) at JNTU-H Kukatpally.
            </p>
        </section>

        <!-- Professional Experience Section -->
        <section id="experience">
            <h2 class="text-2xl md:text-3xl font-bold text-gray-800 mb-4 section-heading">Professional Experience</h2>
            <div class="space-y-6">
                <!-- JNTU-H Kukatpally -->
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">Assistant Professor (temporary)</h3>
                    <p class="text-sm md:text-base text-gray-500">JNTU-H Kukatpally (Jan 2025 - Present)</p>
                    <p class="text-sm md:text-base mt-2 text-gray-600">Subjects taught: Process engineering principles, Chemical Reaction Engineering Lab, Enzyme engineering Lab.</p>
                </div>
                <!-- Riss InfoTech -->
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">Business Development & Sales Manager</h3>
                    <p class="text-sm md:text-base text-gray-500">Riss InfoTech (Jul 2023 - Aug 2023)</p>
                    <ul class="list-disc list-outside mt-2 text-sm md:text-base text-gray-600 space-y-1">
                        <li>Maintained 70 employee database in CRM software.</li>
                        <li>Conducted digital marketing for lead generation and scheduled client meetings.</li>
                        <li>Handled payroll generation and departmental allocation for employees.</li>
                    </ul>
                </div>
                <!-- Excel Engineering College -->
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">Assistant Professor</h3>
                    <p class="text-sm md:text-base text-gray-500">Excel Engineering College (May 2022 - Nov 2022)</p>
                    <ul class="list-disc list-outside mt-2 text-sm md:text-base text-gray-600 space-y-1">
                        <li>Taught courses including Electrochemical Process Technology and Chemical Reaction Engineering.</li>
                        <li>Served as Placement Co-ordinator, Class Advisor/Mentor, and Hostel Warden.</li>
                    </ul>
                </div>
                 <!-- NIT Warangal Researcher -->
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">Researcher in Chemical Engineering</h3>
                    <p class="text-sm md:text-base text-gray-500">National Institute of Technology Warangal (May 2015 - July 2021)</p>
                    <ul class="list-disc list-outside mt-2 text-sm md:text-base text-gray-600 space-y-1">
                        <li>Conducted research on delignification, process engineering, and process simulation.</li>
                        <li>Specialized in supercapacitors, hydrogen production, and polymer chemistry.</li>
                    </ul>
                </div>
                <!-- JNTU Kukatpally Assistant Professor -->
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">Assistant Professor</h3>
                    <p class="text-sm md:text-base text-gray-500">Jawaharlal Nehru Technological University Kukatpally (Dec 2011 - Apr 2014)</p>
                    <ul class="list-disc list-outside mt-2 text-sm md:text-base text-gray-600 space-y-1">
                        <li>Taught M.Tech courses including Process Engineering Principles and Advanced Transport Phenomenon.</li>
                        <li>Handled labs for Process engineering principles and Bioprocess engineering.</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Education Section -->
        <section id="education">
            <h2 class="text-2xl md:text-3xl font-bold text-gray-800 mb-4 section-heading">Education</h2>
            <div class="space-y-6">
                <!-- Ph.D. -->
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">Ph.D. in Chemical Engineering</h3>
                    <p class="text-sm md:text-base text-gray-500">National Institute of Technology Warangal (Aug 2015 - Mar 2021)</p>
                    <p class="text-sm md:text-base mt-2 text-gray-600">Thesis: "Intensification of delignification from Tectona grandis by acoustic cavitation for development of self-healing corrosion inhibition coatings."</p>
                </div>
                <!-- M.Tech -->
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">M.Tech in Chemical Engineering</h3>
                    <p class="text-sm md:text-base text-gray-500">National Institute of Technology Warangal (Jul 2009 - Jul 2011)</p>
                    <p class="text-sm md:text-base mt-2 text-gray-600">Specialization in "Computer Aided Process Equipment Design."</p>
                </div>
                <!-- B.Tech -->
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">B.Tech in Chemical Engineering</h3>
                    <p class="text-sm md:text-base text-gray-500">Jawaharlal Nehru Technological University Anantapur (Jul 2004 - Jul 2008)</p>
                    <p class="text-sm md:text-base mt-2 text-gray-600">Thesis: "Simulation of large-scale membrane reformers by a two-dimensional model."</p>
                </div>
            </div>
        </section>

        <!-- Publications Section -->
        <section id="publications">
            <h2 class="text-2xl md:text-3xl font-bold text-gray-800 mb-4 section-heading">Publications</h2>
            <div class="space-y-6">
                <p class="text-sm md:text-base text-gray-600">
                    Dr. Sushmitha has a significant number of publications in prestigious journals and conferences. You can view all of them on her Google Scholar profile.
                </p>
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Journals</h3>
                    <ul class="list-disc list-outside space-y-2 text-sm md:text-base text-gray-600">
                        <li>Sushmitha Devadasu, Sourabh, Parag Gogate, Srinath Suranani. "Intensification of delignification of tectona grandis saw dust as sustainable biomass using acoustic cavitational devices." <span class="font-medium italic">Ultrasonication and Sonochemistry</span>, 2020.</li>
                        <li>Sushmitha D, Uday B, Shirish H Sonawane, Srinath S. "Development of Ultrahigh build solid self-healing coatings by silanized lignin Nano capsules." <span class="font-medium italic">Materials today Proceedings Journal</span>, 2021.</li>
                        <li>Sushmitha D, Shirish H Sonawane, Srinath Suranani. "Self-healing Corrosion Inhibition Coatings with PH-Responsive Activity by Incorporation of Nano Cellulose in Two pack epoxy polyamide system." <span class="font-medium italic">Materials today Proceedings Journal</span>, 2021.</li>
                        <li>Sushmitha D, Srinath Suranani. "Thermal Modelling of a High Pressure Autoclave Reactor for Hydrothermal Carbonization." <span class="font-medium italic">Lecture Notes in Mechanical Engineering</span>, 2019.</li>
                        <li>Sushmitha D, Srinath Suranani. "Synthesis, and Characterization of Cellulose Nano fibers, in enhancing the tensile stress properties of paper composites." <span class="font-medium italic">International Journal of Engineering & Technology</span>, 2018.</li>
                        <li>Sushmitha D, Pramod. "Review on simulation of Heat Exchanger Using Aspen Plus Software." <span class="font-medium italic">International Journal of Emerging Trends in Engineering and development</span>, 2014.</li>
                    </ul>
                </div>
                
                <div class="card p-6">
                    <h3 class="text-xl font-semibold text-gray-800 mb-2">Conferences</h3>
                    <ul class="list-disc list-outside space-y-2 text-sm md:text-base text-gray-600">
                        <li>"Synthesis of biodegradable multifunctional cellulose hydrogel produced from tectona grandis." 7th International Conference on Recent Advancements in "Chemical, Environmental & Energy Engineering (RACEEE-2023)."</li>
                        <li>"Comparison of self-healing performance of natural anti-corrosion agents, lignin and cellulose on mild steel." International Conference on Waste Energy and Environment (ICWEE-2021).</li>
                        <li>"Evolvement Of Electric Double Layer Pseudo Capacitor By Self-healing Corrosion Inhibition Of Mild Steel." 18th Annual Session of Chemical Engineering Students Congress SEMCON-2022.</li>
                        <li>"Review on Ultra high build solvent less self-healing coatings." 2nd International Conference on Aspects of Materials Science & Engineering, 2021.</li>
                        <li>"Comparison and Evaluation of corrosion inhibition performance of organic coatings." International Conference on Recent Advances in Materials and chemistry (ICRAMC-2021), 2021.</li>
                        <li>"Lignin Encapsulation by Pickering Emulsion and In-Situ Polymerization for Corrosion Inhibition." Energy and Environmental Technologies for Sustainable Development, 2020.</li>
                        <li>"Synthesis of Eco-Friendly and Multifunctional Lignin Based Cellulose Hydrogel from Tectona Grandis Sawdust." International Conference on Current Research and Approaches in Food Technology - CRAFT 2020.</li>
                        <li>"Investigation of a controlled release rate studies on Benzotriazole Loaded Electrospun Cellulose hallow Nano Fibers." International Conference on Recent Advances in Nanoscience and Nanotechnology, 2019.</li>
                        <li>"Optimization of Hydrothermally treated sawdust using RSM CCD." INCEEE-2019, 2019.</li>
                        <li>"Intensification of enzyme activity using sonochemical approach." INCEEE-2019, 2019.</li>
                        <li>"Thermal Modelling of a high pressure Autoclave Reactor for Hydrothermal Carbonization." International Conference on Numerical Heat transfer and fluid flow, 2018.</li>
                        <li>"Kinetic study of degradation of bagasse hydro char using Thermo gravimetric analysis." 7th International Conference on Solid waste management (ICONSWM 2017).</li>
                        <li>"Microwave assisted alkali-peroxide treated sawdust for delignification and its characterization." 7th International Conference on Solid waste management (ICONSWM) 2017.</li>
                        <li>"Hydrothermal Carbonization of Waste Biomass." IHMTC2017-07-1303, 2017.</li>
                        <li>"Optimization of Microwave assisted delignification process parameters using Response surface methodology, central composite design." RESEARCH CONCLAVE, NITW, 2017.</li>
                        <li>"Ultrasound Assisted Pretreatment for efficient delignification of sawdust using sodium per carbonate." CHEMCON IIT-Madras, 2016.</li>
                        <li>"Simulation of large-scale membrane reformers by a two-dimensional model." FUSION-07, 2007.</li>
                        <li>"Supercritical extraction." TECHNOZION-07, 2007.</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Awards and Recognitions Section -->
        <section id="awards">
            <h2 class="text-2xl md:text-3xl font-bold text-gray-800 mb-4 section-heading">Awards & Recognitions</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="card p-6">
                    <h3 class="font-semibold text-gray-900">Best Paper Award</h3>
                    <p class="text-sm text-gray-500">National Conference, NIT Warangal (2017)</p>
                </div>
                <div class="card p-6">
                    <h3 class="font-semibold text-gray-900">Reviewer for Elsevier Journals</h3>
                    <p class="text-sm text-gray-500">"Renewable Energy" & "Materials Today Proceedings"</p>
                </div>
                <div class="card p-6">
                    <h3 class="font-semibold text-gray-900">All India GATE Exam Qualified</h3>
                    <p class="text-sm text-gray-500">Three times (2009, 2010, 2012)</p>
                </div>
                <div class="card p-6">
                    <h3 class="font-semibold text-gray-900">MHRD Scholarship</h3>
                    <p class="text-sm text-gray-500">During Ph.D. at NIT Warangal</p>
                </div>
                <div class="card p-6">
                    <h3 class="font-semibold text-gray-900">AICTE Fellowship</h3>
                    <p class="text-sm text-gray-500">During M.Tech at NIT Warangal</p>
                </div>
                <div class="card p-6">
                    <h3 class="font-semibold text-gray-900">IICHE & IEI Membership</h3>
                    <p class="text-sm text-gray-500">Associate membership since 2017 and 2023</p>
                </div>
            </div>
        </section>

        <!-- Extracurricular Activities Section -->
        <section id="extracurricular">
            <h2 class="text-2xl md:text-3xl font-bold text-gray-800 mb-4 section-heading">Extracurricular Activities</h2>
            <div class="space-y-6">
                <ul class="list-disc list-outside space-y-2 text-sm md:text-base text-gray-600">
                    <li>Won first prize in games & sports i.e. in Running race at JNTU-College Anantapur during 2k7.</li>
                    <li>Won first prize in Kho-kho at JNTU- Engineering College Anantapur in 2k7.</li>
                    <li>Won merit prize in "Hindi Talent Test" in tenth class.</li>
                    <li>Actively participated in cultural festival events "FUSION-05" "SCHEMCON-06".</li>
                    <li>Bagged National level certificate for participating in "All India Inter school cultural festival" at Bangalore.</li>
                    <li>Certified and badged for collecting money to "Help age India" in third class.</li>
                    <li>Awarded first grade in "All India painting competition" at Chennai (Thapasiya School of arts.) in 2k.</li>
                </ul>
            </div>
        </section>

        <!-- References Section -->
        <section id="references">
            <h2 class="text-2xl md:text-3xl font-bold text-gray-800 mb-4 section-heading">References</h2>
            <div class="space-y-6">
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">S. Srinath</h3>
                    <p class="text-sm md:text-base text-gray-500">Associate Professor & Head, Chemical Engineering, NIT-W</p>
                    <p class="text-sm md:text-base text-gray-600 mt-1">Email: <a href="mailto:Srinath@nitw.ac.in" class="no-link-color">Srinath@nitw.ac.in</a></p>
                </div>
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">Shirish Hari Sonawane</h3>
                    <p class="text-sm md:text-base text-gray-500">Professor, Chemical Engineering, NIT-W</p>
                    <p class="text-sm md:text-base text-gray-600 mt-1">Email: <a href="mailto:Shirish@nitw.ac.in" class="no-link-color">Shirish@nitw.ac.in</a></p>
                </div>
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">Pramod Kumar</h3>
                    <p class="text-sm md:text-base text-gray-500">Retired Professor, Chemical Engineering, CCST, IST, JNTU-H</p>
                    <p class="text-sm md:text-base text-gray-600 mt-1">Email: <a href="mailto:pramodkumarr99@gmail.com" class="no-link-color">pramodkumarr99@gmail.com</a></p>
                </div>
                <div class="card p-6">
                    <h3 class="text-lg md:text-xl font-semibold text-gray-900">K. Anand Kishore</h3>
                    <p class="text-sm md:text-base text-gray-500">Associate Professor, Chemical Engineering, NIT-W</p>
                    <p class="text-sm md:text-base text-gray-600 mt-1">Email: <a href="mailto:kola@nitw.ac.in" class="no-link-color">kola@nitw.ac.in</a></p>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-white shadow-inner mt-12 py-6">
        <div class="container mx-auto px-4 text-center text-gray-500 text-sm">
            <p>&copy; 2025 Dr. D. Sushmitha. All Rights Reserved.</p>
        </div>
    </footer>

</body>
</html>

