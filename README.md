<!DOCTYPE html>
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
        .nav-link.active {
            color: #2C7A7B;
            font-weight: 700;
            border-bottom: 2px solid #2C7A7B;
        }
        .content-section {
            display: none;
            animation: fadeIn 0.8s ease-in-out;
        }
        .content-section.active {
            display: block;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @media (max-width: 768px) {
            .btn {
                padding: 0.75rem 1.5rem;
            }
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <!-- Header -->
    <header class="bg-white/80 backdrop-blur-sm shadow-sm py-4 sticky top-0 z-50">
        <div class="container mx-auto px-6 flex flex-col md:flex-row justify-between items-center">
            <h1 class="text-3xl font-bold">Dr. D. Sushmitha</h1>
            <nav class="flex flex-wrap justify-center md:flex-row md:space-x-6 space-x-2 mt-4 md:mt-0 text-sm md:text-base">
                <a href="#about" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors active" data-target="about">About</a>
                <a href="#experience" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors" data-target="experience">Experience</a>
                <a href="#education" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors" data-target="education">Education</a>
                <a href="#publications" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors" data-target="publications">Publications</a>
                <a href="#skills" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors" data-target="skills">Skills</a>
                <a href="#contact" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors" data-target="contact">Contact</a>
            </nav>
        </div>
    </header>

    <!-- Main Content -->
    <main class="flex-grow">
        <div class="container mx-auto px-6 py-12">
            <!-- About Section -->
            <section id="about" class="content-section active">
                <div class="text-center md:flex md:items-center md:text-left mb-16">
                    <div class="md:w-1/3 flex justify-center mb-8 md:mb-0 md:mr-12">
                        <img src="https://placehold.co/250x250/2C7A7B/fff?text=Dr.+Sushmitha" alt="Dr. D. Sushmitha" class="profile-picture w-48 h-48 md:w-64 md:h-64 object-cover">
                    </div>
                    <div class="md:w-2/3">
                        <h2 class="text-5xl md:text-6xl font-extrabold text-gray-900 leading-tight">Hello</h2>
                        <h3 class="text-2xl font-semibold mt-4 text-accent">A Bit About Me</h3>
                        <p class="mt-4 text-gray-700 max-w-xl mx-auto md:mx-0 leading-relaxed">
                            I am a dedicated professional with **over 10 years and 7 months of diverse expertise**, including time as a faculty member, researcher, and manager. My skills span **Process Intensification**, Sustainable Biomass Valorisation, Advanced Coatings, and Process Simulation. I am passionate about leveraging my knowledge for innovation and academic excellence.
                        </p>
                        <div class="flex justify-center md:justify-start space-x-4 mt-8">
                            <a href="#publications" class="btn btn-projects" data-target="publications">Projects</a>
                            <a href="#contact" class="btn btn-contact" data-target="contact">Contact</a>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Experience Section -->
            <section id="experience" class="content-section">
                <h2 class="text-3xl font-bold section-heading">Professional Experience</h2>
                <div class="space-y-4">
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">Assistant Professor (Temporary)</h3>
                        <p class="text-gray-600 text-sm mt-1">Biotechnology Department, IST, JNTU-H | Jan 2025 - Present</p>
                        <ul class="list-disc list-inside mt-2 text-gray-700 text-sm space-y-1">
                            <li>Teaching Process Engineering Principles.</li>
                            <li>Conducting labs for Chemical Reaction Engineering and Enzyme Engineering.</li>
                        </ul>
                    </div>
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">Business Development & Sales Manager</h3>
                        <p class="text-gray-600 text-sm mt-1">Riss InfoTech | Jul 2023 - Aug 2023</p>
                        <ul class="list-disc list-inside mt-2 text-gray-700 text-sm space-y-1">
                            <li>Managed a database of 70 employees using CRM software.</li>
                            <li>Executed digital marketing strategies and managed client relationships.</li>
                            <li>Handled HR duties, including payroll generation.</li>
                        </ul>
                    </div>
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">Assistant Professor</h3>
                        <p class="text-gray-600 text-sm mt-1">Petrochemical Technology, Excel Engineering College | May 2022 - Nov 2022</p>
                        <ul class="list-disc list-inside mt-2 text-gray-700 text-sm space-y-1">
                            <li>Taught courses including Electrochemical Process Technology and Chemical Reaction Engineering.</li>
                            <li>Held key academic roles such as Placement Co-ordinator and Hostel Warden.</li>
                        </ul>
                    </div>
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">Researcher (Ph.D.)</h3>
                        <p class="text-gray-600 text-sm mt-1">National Institute of Technology Warangal (NIT-W) | May 2015 - Jul 2021</p>
                        <ul class="list-disc list-inside mt-2 text-gray-700 text-sm space-y-1">
                            <li>Researched process development for delignification intensification.</li>
                            <li>Utilized ASPEN plus, ASPEN Hysis, and ANSYS for simulation and optimization.</li>
                        </ul>
                    </div>
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">Assistant Professor</h3>
                        <p class="text-gray-600 text-sm mt-1">Biotechnology Department, IST, JNTU-H | Dec 2011 - Apr 2014</p>
                        <ul class="list-disc list-inside mt-2 text-gray-700 text-sm space-y-1">
                            <li>Taught M.Tech courses and handled labs for Process and Bioprocess Engineering.</li>
                        </ul>
                    </div>
                </div>
            </section>

            <!-- Education Section -->
            <section id="education" class="content-section">
                <h2 class="text-3xl font-bold section-heading">Educational Qualifications</h2>
                <div class="space-y-4">
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">Ph.D. in Chemical Engineering</h3>
                        <p class="text-gray-600 text-sm mt-1">National Institute of Technology Warangal | Aug 2015 - Mar 2021</p>
                        <p class="mt-2 text-gray-700 text-sm">Thesis: "Intensification of delignification from *Tectona grandis* by acoustic cavitation for development of self-healing corrosion inhibition coatings."</p>
                    </div>
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">M.Tech in Chemical Engineering</h3>
                        <p class="text-gray-600 text-sm mt-1">National Institute of Technology Warangal | Jul 2009 - Jul 2011</p>
                        <p class="mt-2 text-gray-700 text-sm">Specialization: Computer Aided Process Equipment Design.</p>
                    </div>
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">B.Tech in Chemical Engineering</h3>
                        <p class="text-gray-600 text-sm mt-1">Jawaharlal Nehru Technological University Anantapur | Jul 2004 - Jul 2008</p>
                        <p class="mt-2 text-gray-700 text-sm">Thesis on the simulation of large-scale membrane reformers.</p>
                    </div>
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">GATE Qualified</h3>
                        <p class="text-gray-600 text-sm mt-1">Qualified three times (2009, 2010, 2012) with a highest rank of 1219.</p>
                    </div>
                </div>
            </section>

            <!-- Publications Section -->
            <section id="publications" class="content-section">
                <h2 class="text-3xl font-bold section-heading">Publications & Achievements</h2>
                <div class="space-y-4">
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">Journal Publications (Select)</h3>
                        <ul class="list-disc list-inside mt-2 text-gray-700 text-sm space-y-1">
                            <li>"Intensification of delignification of *Tectona grandis* saw dust as sustainable biomass using acoustic cavitational devices" - **Ultrasonication and Sonochemistry**, 2020.</li>
                            <li>"Development of Ultrahigh build solid self-healing coatings by silanized lignin Nano capsules" - **Materials today Proceedings Journal**, 2021.</li>
                            <li>"Self-healing Corrosion Inhibition Coatings with PH-Responsive Activity..." - **Materials today Proceedings Journal**, 2021.</li>
                        </ul>
                    </div>
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">Awards & Recognition</h3>
                        <ul class="list-disc list-inside mt-2 text-gray-700 text-sm space-y-1">
                            <li>Recipient of the **Best Paper Award** at the "Research Conclave-17" (2017).</li>
                            <li>Official Reviewer for three Elsevier journals.</li>
                            <li>Awarded **MHRD Scholarship** and **AICTE Fellowship**.</li>
                            <li>Associate Member of **IICHE** and **IEI**.</li>
                        </ul>
                    </div>
                </div>
            </section>

            <!-- Skills Section -->
            <section id="skills" class="content-section">
                <h2 class="text-3xl font-bold section-heading">Skills & Expertise</h2>
                <div class="space-y-4">
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">Technical Skills</h3>
                        <ul class="list-disc list-inside mt-2 text-gray-700 text-sm space-y-1">
                            <li>**Software:** ASPEN plus, ASPEN Hysis, ANSYS (3D Modeling), CRM.</li>
                            <li>**Research:** Process Intensification, Biorefinery, Advanced Coatings, Supercapacitors.</li>
                            <li>**Techniques:** Hydrodynamic/Acoustic cavitation, Polarization, EIS.</li>
                        </ul>
                    </div>
                    <div class="card p-4">
                        <h3 class="text-xl font-semibold text-gray-800">Professional Skills</h3>
                        <ul class="list-disc list-inside mt-2 text-gray-700 text-sm space-y-1">
                            <li>**Management:** Business Development, Digital Marketing, HR.</li>
                            <li>**Academic:** Placement Coordination, Mentoring, Hostel Warden.</li>
                        </ul>
                    </div>
                </div>
            </section>

            <!-- Contact Section -->
            <section id="contact" class="content-section">
                <h2 class="text-3xl font-bold section-heading">Contact & Profiles</h2>
                <div class="card p-4">
                    <p class="text-gray-700 text-sm">Feel free to reach out for research collaborations or inquiries.</p>
                    <div class="mt-4 grid md:grid-cols-2 gap-4 text-sm">
                        <div>
                            <p class="font-semibold">Phone</p>
                            <a href="tel:7981541047" class="text-gray-600 block mt-1">7981541047</a>
                            <a href="tel:6304608610" class="text-gray-600 block">6304608610</a>
                        </div>
                        <div>
                            <p class="font-semibold">Email</p>
                            <a href="mailto:Sushmitha.jntu@gmail.com" class="text-gray-600 block mt-1">Sushmitha.jntu@gmail.com</a>
                            <a href="mailto:sushmitha.d.nitw@gmail.com" class="text-gray-600 block">sushmitha.d.nitw@gmail.com</a>
                        </div>
                    </div>
                    <div class="mt-4">
                        <p class="font-semibold">Online Profiles</p>
                        <a href="https://scholar.google.com/citations?user=Qk1uTQYAAAAJ" target="_blank" class="text-blue-500 hover:underline">Google Scholar</a><br>
                        <a href="https://orcid.org/0000-0002-1125-6904" target="_blank" class="text-blue-500 hover:underline">ORCID ID</a>
                    </div>
                </div>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-white shadow-inner py-4 mt-8">
        <div class="container mx-auto px-6 text-center text-gray-600 text-sm">
            <p>&copy; 2023 Dr. D. Sushmitha. All rights reserved.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const navLinks = document.querySelectorAll('.nav-link');
            const sections = document.querySelectorAll('.content-section');
            
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

            navLinks.forEach(link => {
                link.addEventListener('click', (e) => {
                    e.preventDefault();
                    const targetId = e.currentTarget.getAttribute('data-target');
                    showSection(targetId);
                    setActiveLink(targetId);
                    window.history.pushState(null, '', `#${targetId}`);
                });
            });

            const initialSection = window.location.hash.substring(1) || 'about';
            showSection(initialSection);
            setActiveLink(initialSection);
        });
    </script>

</body>
</html>
