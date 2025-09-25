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
            /* Reduced vertical padding (py-3) for smaller height */
            padding: 0.75rem 1rem; 
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
        }
        .btn {
            padding: 0.75rem 2rem;
            border-radius: 9999px;
            font-weight: 600;
            transition: transform 0.2s ease;
        }
        .btn:hover {
            transform: scale(1.03);
        }
        .btn-projects { background-color: #FF5A5F; color: #fff; }
        .btn-contact { background-color: #4CAF50; color: #fff; }
        .text-accent { color: #2C7A7B; }
        .section-heading {
            border-bottom: 2px solid #e2e8f0;
            padding-bottom: 0.5rem;
            margin-bottom: 1rem;
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
            max-height: calc(100vh - 160px); /* Restrict height to reduce scrolling */
            overflow-y: auto; /* Enable internal scrolling if content overflows */
            padding-right: 15px; /* Space for scrollbar */
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
            margin-top: 0.25rem;
        }
        .card ul li {
            margin-bottom: 0.1rem;
            line-height: 1.3;
        }
        .card h3 {
            margin-bottom: 0.1rem;
        }
    </style>
</head>
<body class="flex flex-col min-h-screen">

    <header class="bg-white/80 backdrop-blur-sm shadow-sm py-4 sticky top-0 z-50">
        <div class="container mx-auto px-6 flex flex-col md:flex-row justify-between items-center">
            <h1 class="text-3xl font-bold">Dr. D. Sushmitha</h1>
            <nav class="flex flex-wrap justify-center md:flex-row md:space-x-6 space-x-2 mt-4 md:mt-0 text-sm md:text-base">
                <a href="#about" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors active" data-target="about">Home</a>
                <a href="#experience" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors" data-target="experience">Experience</a>
                <a href="#education" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors" data-target="education">Education</a>
                <a href="#publications" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors" data-target="publications">Research</a>
                <a href="#skills" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors" data-target="skills">Skills</a>
                <a href="#contact" class="nav-link py-2 px-3 text-gray-600 hover:text-gray-900 transition-colors" data-target="contact">Contact</a>
            </nav>
        </div>
    </header>

    <main class="flex-grow">
        <div class="container mx-auto px-6 py-8">
            <section id="about" class="content-section active">
                <div class="text-center md:flex md:items-center md:text-left">
                    <div class="md:w-1/3 flex justify-center mb-6 md:mb-0 md:mr-10">
                        <img src="https://placehold.co/250x250/2C7A7B/fff?text=Dr.+Sushmitha" alt="Dr. D. Sushmitha" class="profile-picture w-40 h-40 md:w-56 md:h-56 object-cover">
                    </div>
                    <div class="md:w-2/3">
                        <h2 class="text-4xl md:text-5xl font-extrabold text-gray-900 leading-tight">Academician & Chemical Engineer</h2>
                        <h3 class="text-xl font-semibold mt-3 text-accent">Over 10 Years of Diverse Expertise</h3>
                        <p class="mt-3 text-gray-700 max-w-xl mx-auto md:mx-0 leading-relaxed text-base">
                            I bring **10 years and 7 months of professional experience** in academia, research, and industry management. My core competence lies in **Process Intensification, Sustainable Biomass Valorisation, Advanced Coatings**, and process simulation using tools like **ASPEN Hysis** and **ANSYS**.
                        </p>
                        <div class="flex justify-center md:justify-start space-x-3 mt-5">
                            <a href="#publications" class="btn btn-projects text-sm" data-target="publications">View Research</a>
                            <a href="#contact" class="btn btn-contact text-sm" data-target="contact">Connect</a>
                        </div>
                    </div>
                </div>
            </section>

            <section id="experience" class="content-section">
                <h2 class="text-3xl font-bold section-heading">Professional Experience</h2>
                <div class="grid md:grid-cols-2 gap-4">
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Assistant Professor (Temporary)</h3>
                        <p class="text-gray-600 text-xs mt-1">Biotechnology, IST, JNTU-H | Jan 2025 - Present</p>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Teaching Process Engineering Principles (B.Tech & M.Sc).</li>
                            <li>Labs: Chemical Reaction Engineering; Enzyme Engineering.</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Assistant Professor</h3>
                        <p class="text-gray-600 text-xs mt-1">Petrochemical Technology, Excel Engineering College | May 2022 - Nov 2022</p>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Courses: Electrochemical Process Tech., Chemical Reaction Engg. I & II, Catalytic Reaction Engg., Fluid Mechanics.</li>
                            <li>Roles: Placement Co-ordinator, Hostel Warden, Internship Co-ordinator.</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Business Development & Sales Manager</h3>
                        <p class="text-gray-600 text-xs mt-1">Riss InfoTech | Jul 2023 - Aug 2023</p>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Managed 70 employees in CRM.</li>
                            <li>Executed Digital Marketing for Lead generation.</li>
                            <li>Handled HR duties, including payroll generation.</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Researcher (Ph.D.)</h3>
                        <p class="text-gray-600 text-xs mt-1">National Institute of Technology Warangal (NIT-W) | May 2015 - Jul 2021</p>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Research focused on Process Intensification (delignification).</li>
                            <li>Software used: ASPEN plus, ASPEN tasc+, ASPEN Hysis, and ANSYS (3D Modeling).</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Assistant Professor</h3>
                        <p class="text-gray-600 text-xs mt-1">Biotechnology, IST, JNTU-H | Dec 2011 - Apr 2014</p>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>M.Tech Courses: Process Engineering Principles, Advanced Transport Phenomenon, Bioprocess Modelling.</li>
                            <li>Labs: Process Engineering Principles; Bioprocess Engineering.</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Industrial Training/Internships</h3>
                        <p class="text-gray-600 text-xs mt-1">Vizag Steel Plant, KERBS, Indo American Pharmaceuticals | 2007-2011</p>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Experience in equipment, process, and bulk drug production.</li>
                        </ul>
                    </div>
                </div>
            </section>

            <section id="education" class="content-section">
                <h2 class="text-3xl font-bold section-heading">Educational Qualifications</h2>
                <div class="grid md:grid-cols-2 gap-4">
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Ph.D. in Chemical Engineering</h3>
                        <p class="text-gray-600 text-xs mt-1">National Institute of Technology Warangal (NIT-W) | Aug 2015 - Mar 2021</p>
                        <p class="mt-1 text-gray-700 text-xs">Thesis on Acoustic Cavitation for Self-Healing Corrosion Inhibition Coatings.</p>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">M.Tech in Chemical Engineering</h3>
                        <p class="text-gray-600 text-xs mt-1">National Institute of Technology Warangal (NIT-W) | Jul 2009 - Jul 2011</p>
                        <p class="mt-1 text-gray-700 text-xs">Specialization: Computer Aided Process Equipment Design (CGPA: 7.28).</p>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">B.Tech in Chemical Engineering</h3>
                        <p class="text-gray-600 text-xs mt-1">Jawaharlal Nehru Technological University Anantapur (JNTU-A) | Jul 2004 - Jul 2008</p>
                        <p class="mt-1 text-gray-700 text-xs">Aggregate: 67.56%.</p>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Academic Achievements</h3>
                        <p class="text-gray-600 text-xs mt-1">Pre-University & Standard</p>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Intermediate (M.P.C): 83.7%.</li>
                            <li>Matriculation (SSC): 80.3%.</li>
                        </ul>
                    </div>
                    <div class="card md:col-span-2">
                        <h3 class="text-base font-semibold text-gray-800">GATE & Fellowships</h3>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Qualified **GATE three times** (2009, 2010, 2012); Highest Rank: 1219 (70.27%).</li>
                            <li>Awarded **MHRD Scholarship** (Ph.D.) and **AICTE Fellowship** (M.Tech).</li>
                        </ul>
                    </div>
                </div>
            </section>

            <section id="publications" class="content-section">
                <h2 class="text-3xl font-bold section-heading">Research, Publications & Recognitions</h2>
                <div class="grid md:grid-cols-2 gap-4">
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Key Journal Publications (6 Total)</h3>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>*Intensification of delignification...* - **Ultrasonication and Sonochemistry** (IF: 9.336).</li>
                            <li>*Development of Ultrahigh build solid self-healing coatings...* - **Materials today Proceedings**.</li>
                            <li>*Self-healing Corrosion Inhibition Coatings with PH-Responsive Activity...* - **Materials today Proceedings**.</li>
                            <li>*Thermal Modelling of a High Pressure Autoclave Reactor...* - **Lecture Notes in Mechanical Engineering**.</li>
                            <li>*Review on simulation of Heat Exchanger Using Aspen Plus...* - **Int. J. Emerging Trends in Engg. and Dev**.</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Conferences & Chapters</h3>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Total: **15 International** and **4 National** Conference Papers.</li>
                            <li>**2 Book Chapters** published.</li>
                        </ul>
                    </div>
                    <div class="card md:col-span-2">
                        <h3 class="text-base font-semibold text-gray-800">Awards & Professional Roles</h3>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Recipient of the **Best Paper Award** at the "Research Conclave-17," NIT Warangal (2017).</li>
                            <li>Official **Reviewer for three Elsevier journals**: *Renewable Energy*, *Materials Today Proceedings*, *Journal of King Saud University - Engg. Science*.</li>
                            <li>Professional Memberships: **Associate Member of IICHE** (since Dec 2017) and **IEI** (since Apr 2023).</li>
                        </ul>
                    </div>
                </div>
            </section>

            <section id="skills" class="content-section">
                <h2 class="text-3xl font-bold section-heading">Skills & Expertise</h2>
                <div class="grid md:grid-cols-2 gap-4">
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Software & Simulation</h3>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Process Simulation & Optimization: **ASPEN plus, ASPEN tasc+, ASPEN Hysis**.</li>
                            <li>Modeling & Analysis: **ANSYS (3D Modeling)**.</li>
                            <li>Business Tools: **CRM Software**.</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Advanced Research Focus</h3>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>**Process Intensification**, Biorefinery, Biomass Valorisation.</li>
                            <li>**New Energy:** Supercapacitors, Electrolytic Hydrogen Production.</li>
                            <li>**Materials:** Self-Healing Coatings, SAP, Multifunctional Hydrogels.</li>
                            <li>**Techniques:** Acoustic/Hydrodynamic Cavitation, EIS.</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Academic & Management</h3>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Curriculum Development, Class Advising, Mentoring.</li>
                            <li>Placement & Internship Coordination, Hostel Warden Duties.</li>
                            <li>Digital Marketing, Lead Generation, Payroll Management.</li>
                        </ul>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Extracurricular Activities</h3>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Won First Prize in Running Race & Kho-kho (JNTU-A, 2k7).</li>
                            <li>First Grade in All India Painting Competition.</li>
                            <li>Certified for collecting money to "Help age India".</li>
                            <li>Assisted in the smooth running of **7 workshops**.</li>
                        </ul>
                    </div>
                </div>
            </section>

            <section id="contact" class="content-section">
                <h2 class="text-3xl font-bold section-heading">Contact & References</h2>
                <div class="grid md:grid-cols-2 gap-4">
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Contact Information</h3>
                        <div class="mt-1 text-sm space-y-1">
                            <p><span class="font-semibold">Phone:</span> 7981541047 / 6304608610</p>
                            <p><span class="font-semibold">Email 1:</span> <a href="mailto:Sushmitha.jntu@gmail.com" class="text-blue-600">Sushmitha.jntu@gmail.com</a></p>
                            <p><span class="font-semibold">Email 2:</span> <a href="mailto:sushmitha.d.nitw@gmail.com" class="text-blue-600">sushmitha.d.nitw@gmail.com</a></p>
                        </div>
                    </div>
                    <div class="card">
                        <h3 class="text-base font-semibold text-gray-800">Online Profiles</h3>
                        <div class="mt-1 text-sm space-y-1">
                            <p><span class="font-semibold">Google Scholar:</span> <a href="https://scholar.google.com/citations?user=Qk1uTQYAAAAJ" target="_blank" class="text-blue-600 hover:underline">View Profile</a></p>
                            <p><span class="font-semibold">ORCID ID:</span> <a href="https://orcid.org/0000-0002-1125-6904" target="_blank" class="text-blue-600 hover:underline">0000-0002-1125-6904</a></p>
                            <p><span class="font-semibold">Scopus ID:</span> 57213192955</p>
                        </div>
                    </div>
                    <div class="card md:col-span-2">
                        <h3 class="text-base font-semibold text-gray-800">References</h3>
                        <p class="mt-1 text-gray-700 text-xs">Available upon request from the following contacts:</p>
                        <ul class="list-disc list-inside mt-1 text-gray-700 text-xs space-y-0">
                            <li>Dr. S. Srinath (Associate Prof & Head, Chemical Engg, NIT-W)</li>
                            <li>Dr. Shirish Hari Sonawane (Professor, Chemical Engg, NIT-W)</li>
                            <li>Dr. K. Anand Kishore (Rtd Professor, Chemical Engg, NIT-W)</li>
                            <li>Dr. Pramod Kumar (Professor, Chemical Engg, CCST, IST, JNTU-H)</li>
                        </ul>
                    </div>
                </div>
            </section>
        </div>
    </main>

    <footer class="bg-white shadow-inner py-4 mt-4">
        <div class="container mx-auto px-6 text-center text-gray-600 text-xs">
            <p>&copy; 2023 Dr. D. Sushmitha. All rights reserved.</p>
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
