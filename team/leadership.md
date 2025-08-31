---
layout: page
permalink: /team/leadership/
leaders:
    - name: Dr. Sanjiva Weerawarana
      position: Founder & Chairman
      start_date: 2023
      image: assets/images/people/Sanjiva_Weerawarana.jpeg
      shortbio:
        In his role as the chairman of LSF, Sanjiva is responsible for guiding
        its strategy and execution in collaboration with the board of directors.
      
    - name: Thushara Rapurathna
      position: Head of Projects
      start_date: 2025-01-01
      moreinfo: https://www.linkedin.com/in/thushara-ruparathna-554369216/
      image: assets/images/people/Thushara_Ruparathna.jpg
      shortbio:
        Thushara joined LSF as a core part of version 3 of LSF where we started focusing on building specific solutions that help (the Sri Lanka) government digitize themselves. Thushara is responsible for managing all the LSF projects
        and also all operational matters of LSF.

        Prior to joining LSF, he was at the Department of Immigration & Emigration of the Sri Lanka government where he was the Deputy Information Technology Controller.

    - name: Nuwan Senaratne
      position: Project Lead for Silver (Volunteer)
      start_date: 2025-01-01
      moreinfo: https://lk.linkedin.com/in/nuwansenaratna
      projects: [Silver]
      image: assets/images/people/Nuwan_Senaratne.jpg
      shortbio: 
        Nuwan is a computer scientist specialising in Artificial Intelligence, Machine Learning, and Data Science. He is an angel investor focused on high-IP AI startups, and a consultant and architect to companies across the US, EU, East Asia, and Sri Lanka. His work spans identifying AI-driven business opportunities, designing intelligent systems, and building high-performing AI teams.

        From 2009 to 2017, he was a Software Engineer and Engineering Manager at Facebook.

        He holds a Master’s in AI, with Distinction in Research, from Stanford University, and a degree from the University of Colombo. He also holds the Licentiate of the Royal Schools of Music (LRSM) in Piano Performance, awarded by the Royal Schools of Music, UK.

    - name: Nayana Samaranayake
      position: Project Lead for OpenDIF (Volunteer)
      start_date: 2025-06-01
      moreinfo: https://www.linkedin.com/in/nayana-samaranayake-ba7b0230/
      projects: [OpenDIF]
      image: assets/images/people/Nayana_Samaranayake.jpg
      shortbio: 
        Nayana is passionate about making a positive impact globally through his experience in technology, management, building non-profit organizations, entrepreneurship. 18+ years of industry experience working for Snapchat in core product, Google in the core search, started two non-profits and multiple technology startup ventures.


---

# Leadership Team

The LSF leadership team are the people who manage day to day operations of LSF. 

<table>
    {% for person in page.leaders %}
        <tr>
            <td width="20%" style="vertical-align: top;">
                <img src="{{ site.baseurl }}/{{ person.image }} " width="100%">
            </td>
            <td>
                <p>
                    <b> {{ person.name }} </b><br>
                    Position: <b> {{ person.position }} </b><br>
                    {{ person.shortbio | markdownify }}
                    {% if person.moreinfo != nil %}
                        More: 
                        <a href="{{ person.moreinfo }}"> {{ person.moreinfo}} </a>
                    {% endif %}
                </p>                
            </td>
        </tr>
    {% endfor %}
</table>
