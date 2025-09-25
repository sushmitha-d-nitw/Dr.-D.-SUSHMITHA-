<html lang="en">
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f4f8;
            color: #333;
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
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
        }
        .btn {
            padding: 1rem 2.5rem;
            border-radius: 9999px;
            font-weight: 600;
            transition: transform 0.2s ease;
        }
        .btn:hover {
            transform: scale(1.05);
        }
        .btn-resume { background-color: #F5A623; color: #333; }
        .btn-projects { background-color: #FF5A5F; color: #fff; }
        .btn-contact { background-color: #4CAF50; color: #fff; }
        .text-accent { color: #2C7A7B; }
        .section-heading {
            border-bottom: 2px solid #e2e8f0;
            padding-bottom: 0.5rem;
            margin-bottom: 1.5rem;
            color: #1a202c;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <!-- Header -->
    <header class="bg-white/80 backdrop-blur-sm shadow-sm py-4 sticky top-0 z-50">
        <div class="container mx-auto px-6 flex justify-between items-center">
            <h1 class="text-2xl font-bold">Dr. D. Sushmitha</h1>
            <nav class="hidden md:flex space-x-6">
                <a href="#about" class="text-gray-600 hover:text-gray-900 transition-colors">About</a>
                <a href="#experience" class="text-gray-600 hover:text-gray-900 transition-colors">Experience</a>
                <a href="#education" class="text-gray-600 hover:text-gray-900 transition-colors">Education</a>
                <a href="#publications" class="text-gray-600 hover:text-gray-900 transition-colors">Publications</a>
                <a href="#skills" class="text-gray-600 hover:text-gray-900 transition-colors">Skills</a>
                <a href="#contact" class="text-gray-600 hover:text-gray-900 transition-colors">Contact</a>
            </nav>
        </div>
    </header>

    <!-- Main Content -->
    <main class="flex-grow">
        <div class="container mx-auto px-6 py-12">
            <!-- Hero Section -->
            <section id="about" class="text-center md:flex md:items-center md:text-left mb-16">
                <div class="md:w-1/3 flex justify-center mb-8 md:mb-0 md:mr-12">
                    <img src="https://placehold.co/250x250/2C7A7B/fff?text=Dr.+Sushmitha" alt="Dr. D. Sushmitha" class="profile-picture w-48 h-48 md:w-64 md:h-64 object-cover">
                </div>
                <div class="md:w-2/3">
                    <h2 class="text-5xl md:text-6xl font-extrabold text-gray-900 leading-tight">Hello</h2>
                    <h3 class="text-2xl font-semibold mt-4 text-accent">A Bit About Me</h3>
                    <p class="mt-4 text-gray-700 max-w-xl mx-auto md:mx-0 leading-relaxed">
                        I am a dedicated professional with over **10 years and 7 months of diverse experience** as a faculty member, researcher, and manager. My expertise spans Process Intensification, Sustainable Biomass Valorisation, Advanced Coatings, and Process Simulation. I am passionate about leveraging my skills to drive innovation and academic excellence.
                    </p>
                    <div class="flex justify-center md:justify-start space-x-4 mt-8">
                        <a href="#publications" class="btn btn-projects">Projects</a>
                        <a href="#contact" class="btn btn-contact">Contact</a>
                    </div>
                </div>
            </section>

            <!-- Experience Section -->
            <section id="experience" class="mb-12">
                <h2 class="text-3xl font-bold section-heading">Professional Experience</h2>
                <div class="space-y-8">
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Assistant Professor (Temporary)</h3>
                        <p class="text-gray-600 mt-1">Biotechnology Department, IST, JNTU-H | Jan 2025 - Present</p>
                        <ul class="list-disc list-inside mt-4 text-gray-700 space-y-2">
                            <li>Teaching Process Engineering Principles to B.Tech and M.Sc students.</li>
                            <li>Conducting labs for Chemical Reaction Engineering and Enzyme Engineering.</li>
                        </ul>
                    </div>
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Assistant Professor</h3>
                        <p class="text-gray-600 mt-1">Petrochemical Technology Department, Excel Engineering College | May 2022 - Nov 2022</p>
                        <ul class="list-disc list-inside mt-4 text-gray-700 space-y-2">
                            <li>Instructed various courses including Electrochemical Process Technology, Chemical Reaction Engineering, and Fluid Mechanics.</li>
                            <li>Held key academic roles such as Placement Co-ordinator, Class Advisor, and Hostel Warden.</li>
                        </ul>
                    </div>
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Business Development & Sales Manager</h3>
                        <p class="text-gray-600 mt-1">Riss InfoTech | Jul 2023 - Aug 2023</p>
                        <ul class="list-disc list-inside mt-4 text-gray-700 space-y-2">
                            <li>Managed a database of 70 employees using CRM software.</li>
                            <li>Executed digital marketing strategies for lead generation and managed client relationships.</li>
                            <li>Handled HR duties, including payroll generation and department allocation.</li>
                        </ul>
                    </div>
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Researcher (Ph.D.)</h3>
                        <p class="text-gray-600 mt-1">National Institute of Technology Warangal (NIT-W) | May 2015 - Jul 2021</p>
                        <ul class="list-disc list-inside mt-4 text-gray-700 space-y-2">
                            <li>Conducted research on process development for delignification intensification.</li>
                            <li>Utilized software like ASPEN plus, ASPEN Hysis, and ANSYS for simulation and optimization.</li>
                        </ul>
                    </div>
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Assistant Professor</h3>
                        <p class="text-gray-600 mt-1">Biotechnology Department, IST, JNTU-H | Dec 2011 - Apr 2014</p>
                        <ul class="list-disc list-inside mt-4 text-gray-700 space-y-2">
                            <li>Taught M.Tech courses in Process Engineering, Transport Phenomenon, and Bioprocess Modeling.</li>
                            <li>Managed labs for Process and Bioprocess Engineering.</li>
                        </ul>
                    </div>
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Industrial Training</h3>
                        <p class="text-gray-600 mt-1">Vizag Steel Plant, KERBS Kavali, and Indo American Pharmaceuticals | 2007-2011</p>
                        <ul class="list-disc list-inside mt-4 text-gray-700 space-y-2">
                            <li>Gained hands-on experience in equipment, processes, and bulk drug production.</li>
                        </ul>
                    </div>
                </div>
            </section>

            <!-- Education Section -->
            <section id="education" class="mb-12">
                <h2 class="text-3xl font-bold section-heading">Educational Qualifications</h2>
                <div class="space-y-8">
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Ph.D. in Chemical Engineering</h3>
                        <p class="text-gray-600 mt-1">National Institute of Technology Warangal | Aug 2015 - Mar 2021</p>
                        <p class="mt-2 text-gray-700">Thesis: "Intensification of delignification from Tectona grandis by acoustic cavitation for development of self-healing corrosion inhibition coatings."</p>
                    </div>
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">M.Tech in Chemical Engineering</h3>
                        <p class="text-gray-600 mt-1">National Institute of Technology Warangal | Jul 2009 - Jul 2011</p>
                        <p class="mt-2 text-gray-700">Specialization: Computer Aided Process Equipment Design. Thesis on improving crude benzol production using Aspen.</p>
                    </div>
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">B.Tech in Chemical Engineering</h3>
                        <p class="text-gray-600 mt-1">Jawaharlal Nehru Technological University Anantapur | Jul 2004 - Jul 2008</p>
                        <p class="mt-2 text-gray-700">Thesis on the simulation of large-scale membrane reformers using a two-dimensional model.</p>
                    </div>
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">GATE Qualified</h3>
                        <p class="text-gray-600 mt-1">Qualified three times (2009, 2010, 2012) with a highest rank of 1219.</p>
                    </div>
                </div>
            </section>

            <!-- Publications Section -->
            <section id="publications" class="mb-12">
                <h2 class="text-3xl font-bold section-heading">Publications & Achievements</h2>
                <div class="space-y-8">
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Journal Publications</h3>
                        <ul class="list-disc list-inside mt-4 text-gray-700 space-y-2">
                            <li>"Intensification of delignification of *Tectona grandis* saw dust as sustainable biomass using acoustic cavitational devices" - **Ultrasonication and Sonochemistry**, 2020.</li>
                            <li>"Development of Ultrahigh build solid self-healing coatings by silanized lignin Nano capsules" - **Materials today Proceedings Journal**, 2021.</li>
                            <li>"Self-healing Corrosion Inhibition Coatings with PH-Responsive Activity by Incorporation of Nano Cellulose..." - **Materials today Proceedings Journal**, 2021.</li>
                            <li>"Thermal Modelling of a High Pressure Autoclave Reactor for Hydrothermal Carbonization" - **Lecture Notes in Mechanical Engineering**, 2019.</li>
                            <li>"Review on simulation of Heat Exchanger Using Aspen Plus Software" - **International Journal of Emerging Trends in Engineering and development**, 2014.</li>
                        </ul>
                    </div>
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Awards & Recognition</h3>
                        <ul class="list-disc list-inside mt-4 text-gray-700 space-y-2">
                            <li>Recipient of the **Best Paper Award** at the "Research Conclave-17," NIT Warangal (2017).</li>
                            <li>Official Reviewer for three Elsevier journals: "Renewable Energy," "Materials Today Proceedings," and "Journal of King Saud University."</li>
                            <li>Awarded the **MHRD Scholarship** and **AICTE Fellowship** during Ph.D. and M.Tech studies.</li>
                            <li>Associate Member of the Indian Institute of Chemical Engineers (IICHE) and the Institute of Engineers India (IEI).</li>
                        </ul>
                    </div>
                </div>
            </section>

            <!-- Skills Section -->
            <section id="skills" class="mb-12">
                <h2 class="text-3xl font-bold section-heading">Skills & Expertise</h2>
                <div class="space-y-8">
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Technical Skills</h3>
                        <ul class="list-disc list-inside mt-4 text-gray-700 space-y-2">
                            <li>**Software:** ASPEN plus, ASPEN tasc+, ASPEN Hysis, ANSYS (3D Modeling).</li>
                            <li>**Research:** Process Intensification, Biorefinery, Advanced Coatings, Supercapacitors.</li>
                            <li>**Techniques:** Hydrodynamic/Acoustic cavitation, Polarization, and EIS.</li>
                        </ul>
                    </div>
                    <div class="card p-6">
                        <h3 class="text-2xl font-semibold text-gray-800">Professional Skills</h3>
                        <ul class="list-disc list-inside mt-4 text-gray-700 space-y-2">
                            <li>**Management:** Business Development, Digital Marketing, CRM, HR.</li>
                            <li>**Academic:** Placement Coordination, Mentoring, Class Committee Coordination.</li>
                        </ul>
                    </div>
                </div>
            </section>

            <!-- Contact Section -->
            <section id="contact" class="mb-12">
                <h2 class="text-3xl font-bold section-heading">Contact & Profiles</h2>
                <div class="card p-8 text-center md:text-left">
                    <div class="grid md:grid-cols-2 gap-6">
                        <div>
                            <p class="text-lg font-semibold text-gray-800">Phone</p>
                            <a href="tel:7981541047" class="text-gray-600 block mt-1">7981541047</a>
                            <a href="tel:6304608610" class="text-gray-600 block">6304608610</a>
                        </div>
                        <div>
                            <p class="text-lg font-semibold text-gray-800">Email</p>
                            <a href="mailto:Sushmitha.jntu@gmail.com" class="text-gray-600 block mt-1">Sushmitha.jntu@gmail.com</a>
                            <a href="mailto:sushmitha.d.nitw@gmail.com" class="text-gray-600 block">sushmitha.d.nitw@gmail.com</a>
                        </div>
                    </div>
                    <div class="mt-6 flex flex-col items-center md:items-start space-y-2">
                        <p class="text-lg font-semibold text-gray-800">Online Profiles</p>
                        <a href="https://scholar.google.com/citations?user=Qk1uTQYAAAAJ" target="_blank" class="text-blue-500 hover:underline">Google Scholar</a>
                        <a href="https://orcid.org/0000-0002-1125-6904" target="_blank" class="text-blue-500 hover:underline">ORCID ID: 0000-0002-1125-6904</a>
                        <p class="text-gray-600">Scopus ID: 57213192955</p>
                    </div>
                </div>
            </section>

        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-white shadow-inner py-6 mt-12">
        <div class="container mx-auto px-6 text-center text-gray-600">
            <p>&copy; 2023 Dr. D. Sushmitha. All rights reserved.</p>
        </div>
    </footer>

</body>
</html>
