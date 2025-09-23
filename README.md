<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dr. D. Sushmitha - Professional Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Chosen Palette: Cool Gray & Blue -->
    <!-- Application Structure Plan: The application uses a classic master-detail (sidebar/content) layout. This structure is ideal for presenting a comprehensive academic and professional profile. The sidebar provides a persistent, hierarchical navigation menu for key sections like 'About', 'Professional Experience', 'Education', 'Publications', and 'Awards'. The main content area dynamically updates to show detailed information for each selected section. This design allows users to easily explore the depth and breadth of Dr. Sushmitha's profile without navigating away from the page. This SPA approach ensures a fast and seamless user experience. -->
    <!-- Visualization & Content Choices: The portfolio is information-dense, focusing on academic and professional achievements. The goal is to inform and establish credibility. The primary presentation method is structured HTML with clear headings, lists, and bold text to highlight key information. The content is organized into logical sections based on the resume. The main interaction is the navigation menu, which updates the visible content panel. This is a simple and intuitive way to present a large amount of information. No complex visualizations are necessary, as the data is primarily textual. The interaction is powered by vanilla JavaScript. -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <style>
        .nav-link.active {
            background-color: #3b82f6;
            color: white;
            font-weight: 600;
        }
        .content-panel {
            animation: fadeIn 0.5s ease-in-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 font-sans">

    <div class="container mx-auto max-w-6xl p-4 sm:p-6 lg:p-8">
        
        <header class="pb-6 border-b border-gray-200">
            <h1 class="text-4xl font-bold text-gray-900 tracking-tight">Dr. D. Sushmitha's Professional Profile</h1>
            <p class="mt-2 text-lg text-gray-600">A comprehensive overview of academic, professional, and research experience.</p>
        </header>

        <main class="grid grid-cols-1 md:grid-cols-4 gap-8 mt-8">
            
            <aside class="md:col-span-1">
                <nav class="sticky top-8">
                    <ul class="space-y-2">
                        <li><a href="#" class="nav-link active w-full text-left flex items-center p-3 rounded-lg text-gray-700 hover:bg-gray-100 transition-colors duration-200" data-target="about">About Me</a></li>
                        <li><a href="#" class="nav-link w-full text-left flex items-center p-3 rounded-lg text-gray-700 hover:bg-gray-100 transition-colors duration-200" data-target="experience">Professional Experience</a></li>
                        <li><a href="#" class="nav-link w-full text-left flex items-center p-3 rounded-lg text-gray-700 hover:bg-gray-100 transition-colors duration-200" data-target="education">Educational Qualifications</a></li>
                        <li><a href="#" class="nav-link w-full text-left flex items-center p-3 rounded-lg text-gray-700 hover:bg-gray-100 transition-colors duration-200" data-target="publications">Publications</a></li>
                        <li><a href="#" class="nav-link w-full text-left flex items-center p-3 rounded-lg text-gray-700 hover:bg-gray-100 transition-colors duration-200" data-target="awards">Awards & Recognitions</a></li>
                        <li><a href="#" class="nav-link w-full text-left flex items-center p-3 rounded-lg text-gray-700 hover:bg-gray-100 transition-colors duration-200" data-target="contact">Contact Me</a></li>
                    </ul>
                </nav>
            </aside>

            <section class="md:col-span-3">
                <div class="bg-white p-6 sm:p-8 rounded-xl shadow-sm border border-gray-200">
                    <div id="about" class="content-panel space-y-4">
                        <h2 class="text-3xl font-semibold text-gray-900 border-b pb-3">About Me</h2>
                        <p class="text-gray-600 leading-relaxed">
                            A highly experienced academician and researcher with over 10 years and 7 months of diverse expertise in chemical and biochemical engineering. I am currently an **Assistant Professor (temporary)** at the Biotechnology department, JNTU-H, specializing in **Process Engineering Principles** and related laboratory work. My professional journey includes significant roles as a **Researcher** at the National Institute of Technology Warangal and as a **Business Development Manager** at Riss InfoTech. My research interests are broad, ranging from process intensification and biorefinery to the synthesis of advanced materials like **Supercapacitors** and **self-healing corrosion coatings**. I have a proven track record of teaching and mentorship, coupled with strong project management and leadership skills.
                        </p>
                    </div>

                    <div id="experience" class="content-panel hidden space-y-6">
                        <h2 class="text-3xl font-semibold text-gray-900 border-b pb-3">Professional Experience</h2>
                        <div class="border-l-4 border-blue-500 pl-4">
                            <h3 class="text-xl font-semibold text-gray-800">Assistant Professor (temporary)</h3>
                            <p class="text-gray-600">Biotechnology Department, IST JNTU-H, Kukatpally</p>
                            <p class="text-sm text-gray-500">Jan 2025 - Present</p>
                            <p class="text-gray-600 mt-2">Teaching **Process Engineering Principles** to B.Tech and M.Sc students. Handling labs for **Chemical Reaction Engineering** and **Enzyme Engineering**.</p>
                        </div>
                        <div class="border-l-4 border-blue-500 pl-4">
                            <h3 class="text-xl font-semibold text-gray-800">Business Development & Sales Manager</h3>
                            <p class="text-gray-600">Riss InfoTech</p>
                            <p class="text-sm text-gray-500">July 2023 - Aug 2023</p>
                            <p class="text-gray-600 mt-2">Managed digital marketing, lead generation, and client relationship management. Responsible for employee data, payroll, and department allocation.</p>
                        </div>
                        <div class="border-l-4 border-blue-500 pl-4">
                            <h3 class="text-xl font-semibold text-gray-800">Researcher in Chemical Engineering</h3>
                            <p class="text-gray-600">National Institute of Technology Warangal</p>
                            <p class="text-sm text-gray-500">May 2015 - July 2021</p>
                            <p class="text-gray-600 mt-2">Conducted extensive research on **Process intensification** and **optimization** using **ASPEN Plus**, **ASPEN Hysis**, and **ANSYS**.</p>
                        </div>
                    </div>

                    <div id="education" class="content-panel hidden space-y-6">
                        <h2 class="text-3xl font-semibold text-gray-900 border-b pb-3">Educational Qualifications</h2>
                        <div class="border-l-4 border-blue-500 pl-4">
                            <h3 class="text-xl font-semibold text-gray-800">Ph.D. / Doctor of Philosophy - Chemical Engineering</h3>
                            <p class="text-gray-600">National Institute of Technology Warangal (NIT-W)</p>
                            <p class="text-sm text-gray-500">Aug 2015 - March 2021</p>
                        </div>
                        <div class="border-l-4 border-blue-500 pl-4">
                            <h3 class="text-xl font-semibold text-gray-800">M.Tech / Post Graduate - Chemical Engineering</h3>
                            <p class="text-gray-600">National Institute of Technology Warangal (NIT-W)</p>
                            <p class="text-sm text-gray-500">July 2009 - July 2011</p>
                        </div>
                        <div class="border-l-4 border-blue-500 pl-4">
                            <h3 class="text-xl font-semibold text-gray-800">B.Tech / Graduation - Chemical Engineering</h3>
                            <p class="text-gray-600">Jawaharlal Nehru Technological University Anantapur (JNTU-A)</p>
                            <p class="text-sm text-gray-500">July 2004 - July 2008</p>
                        </div>
                    </div>

                    <div id="publications" class="content-panel hidden space-y-6">
                        <h2 class="text-3xl font-semibold text-gray-900 border-b pb-3">Publications</h2>
                        <p class="text-gray-600">A selection of my published work in journals and conferences.</p>
                        <button id="summarize-btn" class="bg-blue-500 text-white rounded-md px-4 py-2 hover:bg-blue-600 transition-colors duration-200">✨ Summarize Publications</button>
                        <div id="summary-output" class="mt-4 p-4 bg-gray-100 rounded-md hidden"></div>

                        <div class="border-l-4 border-blue-500 pl-4">
                             <h3 class="text-xl font-semibold text-gray-800">Journals</h3>
                             <ul id="journal-list" class="list-disc list-inside text-gray-600 space-y-2 mt-2">
                                 <li>Intensification of delignification of tectona grandis saw dust as sustainable biomass using acoustic cavitational devices.</li>
                                 <li>Development of Ultrahigh build solid self-healing coatings by silanized lignin Nano capsules.</li>
                                 <li>Self-healing Corrosion Inhibition Coatings with PH-Responsive Activity by Incorporation of Nano Cellulose in Two pack epoxy polyamide system.</li>
                             </ul>
                        </div>
                        <div class="border-l-4 border-blue-500 pl-4 mt-6">
                             <h3 class="text-xl font-semibold text-gray-800">International Conferences</h3>
                             <ul id="international-list" class="list-disc list-inside text-gray-600 space-y-2 mt-2">
                                 <li>Synthesis of biodegradable multifunctional cellulose hydrogel produced from tectona grandis.</li>
                                 <li>Comparison of self-healing performance of natural anti-corrosion agents, lignin and cellulose on mild steel.</li>
                                 <li>Evolvement Of Electric Double Layer Pseudo Capacitor By Self-healing Corrosion Inhibition Of Mild Steel.</li>
                             </ul>
                        </div>
                        <div class="border-l-4 border-blue-500 pl-4 mt-6">
                             <h3 class="text-xl font-semibold text-gray-800">National Conferences</h3>
                             <ul id="national-list" class="list-disc list-inside text-gray-600 space-y-2 mt-2">
                                 <li>Optimization of Microwave assisted delignification process parameters using Response surface methodology, central composite design.</li>
                                 <li>Ultrasound Assisted Pretreatment for efficient delignification of sawdust using sodium per carbonate.</li>
                             </ul>
                        </div>
                    </div>

                    <div id="awards" class="content-panel hidden space-y-6">
                        <h2 class="text-3xl font-semibold text-gray-900 border-b pb-3">Awards & Recognitions</h2>
                        <ul class="list-disc list-inside text-gray-600 space-y-2">
                            <li>Best Paper Award in National Conference, Research conclave-17, NITW.</li>
                            <li>Three times qualified in the All India GATE exam (2009, 2010, 2012).</li>
                            <li>Received Scholarship from the Ministry of Human Resources Development (MHRD), Govt. of India during Ph.D.</li>
                            <li>Received AICTE fellowship during M.Tech in Dept., of Chemical Engineering, NIT-W.</li>
                            <li>Reviewer for three Elsevier journals.</li>
                        </ul>
                    </div>

                    <div id="contact" class="content-panel hidden space-y-4">
                        <h2 class="text-3xl font-semibold text-gray-900 border-b pb-3">Contact Me</h2>
                        <p class="text-gray-600">I am open to new opportunities and collaborations. Feel free to reach out using the details below.</p>
                        <ul class="space-y-2 text-gray-700">
                           <li class="flex items-center"><span class="font-semibold w-20">Phone:</span> 7981541047</li>
                           <li class="flex items-center"><span class="font-semibold w-20">Email:</span> <a href="mailto:sushmitha.d.nitw@gmail.com" class="text-blue-500 hover:underline">sushmitha.d.nitw@gmail.com</a></li>
                            <li class="flex items-center"><span class="font-semibold w-20">Google Scholar:</span> <a href="https://scholar.google.com/citations?user=Qk1uTQYAAAAJ" class="text-blue-500 hover:underline">scholar.google.com/citations?user=Qk1uTQYAAAAJ</a></li>
                            <li class="flex items-center"><span class="font-semibold w-20">ORCID ID:</span> <a href="https://orcid.org/0000-0002-1125-6904" class="text-blue-500 hover:underline">orcid.org/0000-0002-1125-6904</a></li>
                        </ul>
                    </div>
                </div>
            </section>
        </main>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const navLinks = document.querySelectorAll('.nav-link');
            const contentPanels = document.querySelectorAll('.content-panel');
            const summarizeBtn = document.getElementById('summarize-btn');
            const summaryOutput = document.getElementById('summary-output');
            const journalList = document.getElementById('journal-list');
            const internationalList = document.getElementById('international-list');
            const nationalList = document.getElementById('national-list');
            
            navLinks.forEach(link => {
                link.addEventListener('click', (event) => {
                    event.preventDefault();
                    navLinks.forEach(nav => nav.classList.remove('active'));
                    contentPanels.forEach(panel => panel.classList.add('hidden'));
                    link.classList.add('active');
                    
                    const targetId = link.dataset.target;
                    const targetPanel = document.getElementById(targetId);
                    if (targetPanel) {
                        targetPanel.classList.remove('hidden');
                    }
                });
            });

            summarizeBtn.addEventListener('click', async () => {
                const publications = [
                    ...Array.from(journalList.children).map(li => li.textContent),
                    ...Array.from(internationalList.children).map(li => li.textContent),
                    ...Array.from(nationalList.children).map(li => li.textContent)
                ].join('; ');

                summaryOutput.innerHTML = 'Generating summary...';
                summaryOutput.classList.remove('hidden');
                
                const prompt = `Act as a scientific writer and generate a professional, single-paragraph summary of the following research publications. Focus on the main themes and contributions.

                Publications: ${publications}`;

                const payload = {
                    contents: [{ parts: [{ text: prompt }] }],
                    model: "gemini-2.5-flash-preview-05-20"
                };

                const apiKey = "";
                const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-05-20:generateContent?key=${apiKey}`;

                let response;
                try {
                    response = await fetch(apiUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });

                    if (!response.ok) {
                        throw new Error(`API error: ${response.status} ${response.statusText}`);
                    }

                    const result = await response.json();
                    const summary = result.candidates?.[0]?.content?.parts?.[0]?.text || "Failed to generate summary.";
                    summaryOutput.innerHTML = `<p class="font-semibold">Summary of Research:</p><p>${summary}</p>`;
                } catch (error) {
                    console.error('Error fetching data from Gemini API:', error);
                    summaryOutput.innerHTML = '<p class="text-red-600">Sorry, an error occurred while generating the summary. Please try again later.</p>';
                }
            });
        });
    </script>

</body>
</html>
