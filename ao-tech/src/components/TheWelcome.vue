<script setup lang="ts">
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
import CvSections from './CvSections.vue'
import CvSectionsExpanded from './CvSectionsExpanded.vue'
import Work from './Work.vue'
import Education from './Education.vue'
import ProfileIcon from './icons/profile.vue'
import WorkIcon from './icons/work.vue'
import EducationIcon from './icons/education.vue'
import Edcucation2Icon from './icons/education2.vue'
import CertificationIcon from './icons/certification.vue'
import CertificationComponent from './Certification.vue'
import GeneralIcon from './icons/general.vue'
import ContactIcon from './icons/contact.vue'

</script>

<template>
  <CvSectionsExpanded>
    <template #icon>
      <ProfileIcon />
    </template>
    <template #heading>Profil</template>
    Andreas Olausson är en motiverad och erfaren utvecklare med bred teknisk erfarenhet inom hela stacken och över 20 år i
    branschen.
    Andreas arbetar gärna agilt och är speciellt intresserad i webb-utveckling, vilket han fördjupat sig med de senaste
    åren. Förutom att Andreas arbetar som ren utvecklare har han erfarenhet i att projektleda mindre utvecklings-projekt
    samt hålla i systemdesign.

  </CvSectionsExpanded>

  <CvSections>
    <template #icon>
      <WorkIcon />
    </template>
    <template #heading>Arbetslivserfarenhet</template>

    <Work>
      <template #header>Senior utvecklare - Frilans</template>
      <template #where>Linköping</template>
      <template #when>September, 2018 -></template>
      <template #what>Webb/System-utveckling av kart-tjänst med Leaflet-karta som utgångspunkt. <br>
        Applikationen vänder sig bland annat till mäklare som kan använda systemet som boll-plank för att exempelvis
        ta fram ett estimerat pris vid en eventuell försäljning av en bostad.
      </template>
      <template #role>Roll: utvecklare, systemdesign/arkitektur</template>
      <template #tech>Teknologi: Typescript, Angular, Leaflet, MVC, ASP.NET, C#, SQL.</template>
    </Work>
    <Work>
      <template #header>Senior utvecklare - Eiendomsverdi AS</template>
      <template #where>Oslo</template>
      <template #when>September 2013 — September 2018</template>
      <template #what>Webb/System-utveckling och underhåll av AVM-applikationer (Automated Valuation Model).</template>
      <template #role>Roll: utvecklare, systemdesign/arkitektur</template>
      <template #tech>Teknologi: C#, ASP.NET, MVC 4, Angular, jQuery, JavaScript, SQL.</template>
    </Work>
    <Work>
      <template #header>Senior konsult - IT-Verket AS</template>
      <template #where>Oslo</template>
      <template #when>Februari 2012 — Juni 2013</template>
      <template #what>Diverse konsultuppdrag inom webb/system-utveckling bland annat:<br>
        Folkehelseinstituttet: Ansvarig för uppgradering av windows-service samt webb-applikationer från .Net 1.1 till
        .Net 4.0.<br>
        Finans Norge: Projektledare och utvecklare av en säkerhetsklassad (klass 4/4) webb-applikation.<br>
        Næringslivets Hovedorganisasjon: Projektledare och utvecklare system för fakturering av medlemar.<br>
        Fearnley Offshore: Utveckling av webb-applikation för underhåll av oljeriggar.</template>
      <template #role>Roll: utvecklare, projektledare</template>
      <template #tech>Teknologi: C#, ASP.NET MVC3/4, NHibernate, NUnit, jQuery, Ajax, SQL, Buypass, FoxPro</template>
    </Work>
    <Work>
      <template #header>Senior konsult - Capra Consulting AS</template>
      <template #where>Oslo</template>
      <template #when>September 2011 — Februari 2012</template>
      <template #what>Konsultuppdrag inom webb/system-utveckling.<br>
        Arkitektur och utveckling av en webb-applikation samt en WCF Webb-service som konsumeras av en
        IPhone-app.</template>
      <template #role>Roll: utvecklare</template>
      <template #tech>Teknologi: C #, SQL Azure, WCF, ASP.NET, Ajax / jQuery, XPath</template>
    </Work>
    <Work>
      <template #header>Senior utvecklare - Solid Park AB</template>
      <template #where>Stockholm</template>
      <template #when>December 2008 — September 2011</template>
      <template #what>Diverse konsultuppdrag inom webb/system-utveckling bland annat:<br>
        Lärarförsäkringar: Utveckling av klientapplikationer för medlemssystem. Utveckling av diverse webbtjänster.<br>
        Lärarförbundet: Utveckling av “LOKA”, medlemsadministration av lokalföreningar och implementation av AID-koder
        (statistik-koder).<br>
        Lärarnas riksförbund: Integration av medlemssystem och katalogtjäster.<br>
        Lärarnas tidningsproduktion: Arkitektur och utveckling av ”Tobias”, en webb-applikation för hantering av bilagor
        vid utskick av tidningar.</template>
      <template #role>Roll: utvecklare, systemdesign/arkitektur</template>
      <template #tech>Teknologi: ASP.NET, C#, SQL, AJAX, JavaScript, jQuery, LDAP, WPF, Web services</template>
    </Work>
    <Work>
      <template #header>Utvecklare - 4GHI Solutions AB</template>
      <template #where>Norrköping</template>
      <template #when>Juli 2005 — December 2008</template>
      <template #what>Utveckling och arkitektur av Cockpit Communicator, ett webbaserat IT-stöd för prestationshantering
        inklusive balanserade styrkort. <br>
        Utveckling av Cocpit Survey, ett enkät-system.</template>
      <template #role>Roll: utvecklare, systemdesign/arkitektur</template>
      <template #tech>Teknologi: ASP, VB, C#, JavaScript, SQL/Oracle</template>
    </Work>
    <Work>
      <template #header>Utvecklare - Frilans</template>
      <template #where>Linköping</template>
      <template #when>Februari 2002 — Maj 2005</template>
      <template #what>Diverse konsultuppdrag inom webb/system-utveckling bland annat:<br>
        Utveckling av klagomålssystem, verktyg för log-analys.<br>
        Utveckling av Hotell-reservationssystem specialiserat för gruppbokningar.<br>
        Databasprogrammering, Export av företagsspecifik information ur större SQL-databas.<br>
        Databasprogrammering, Migrering av CRM-system.
      </template>
      <template #role>Roll: utvecklare</template>
      <template #tech>Teknologi: ASP, Javascript, VB, VB.NET, SQL, Lotus Notes.</template>
    </Work>
    <Work>
      <template #header>Utvecklare - AB Motala Verkstad</template>
      <template #where>Motala</template>
      <template #when>September 2002 — Juli 2004</template>
      <template #what>Utveckling och underhåll av lokalt intranät samt teknisk support.</template>
      <template #role>Roll: utvecklare</template>
      <template #tech>Teknologi: ASP.NET, VB.NET, SQL/DB2</template>
    </Work>
    <Work>
      <template #header>Utvecklare - Scanres Hospitality Solutions AB</template>
      <template #where>Stockholm</template>
      <template #when>Juli 2000 — December 2001</template>
      <template #what>Utveckling av reservationssystem för hotellbokningar och lojalitetsprogram.</template>
      <template #role>Roll: utvecklare</template>
      <template #tech>Teknologi: ASP, VB, SQL</template>
    </Work>

  </CvSections>

  <CvSections>
    <template #icon>
      <EducationIcon />
    </template>
    <template #heading>Utbildning</template>
    <Education>
      <template #header>MCSD - Computer Research</template>
      <template #where>Stockholm</template>
      <template #when>Januari 2000 — Juni 2000</template>
      <template #what>Intensiv certifieringsutbildning för Microsoft Certified Solution Developer</template>
    </Education>
    <Education>
      <template #header>Certified Web Master - Semcon Educations</template>
      <template #where>Stockholm</template>
      <template #when>Januari 1999 - Juni 1999</template>
      <template #what>Certifieringsutbildning för att bli certifierad ”Web Master”.</template>
    </Education>
    <Education>
      <template #header>Web publisher - ALU</template>
      <template #where>Norrköping</template>
      <template #when>Augusti 1997 - Maj 1998</template>
      <template #what>Utbildning inom grafisk design på webben.</template>
    </Education>
    <Education>
      <template #header>KOMVUX - Elsa Brändströms skola</template>
      <template #where>Linköping</template>
      <template #when>Augusti 1996 – Juni 1997</template>
      <template #what>Diverse gymnasieämnen.</template>
    </Education>
    <Education>
      <template #header>Gymnasieskolan - Anders Ljungstedts Skola</template>
      <template #where>Linköping</template>
      <template #when>1996-08 – 1997-06</template>
      <template #what>3-årig ekonomisk linje.</template>
    </Education>
  </CvSections>

  <CvSections>
    <template #icon>
      <Edcucation2Icon />
    </template>
    <template #heading>Kurser</template>
    <Education>
      <template #header>Building Web Apps with Angular - Learningtree</template>
      <template #where>Stockholm</template>
      <template #when>Mars 2017 - Mars 2017</template>
      <template #what>Kurs i angular</template>
    </Education>
    <Education>
      <template #header>CITA-F Architecture Core - Dataförening kompetens</template>
      <template #where>Stockholm</template>
      <template #when>September 2015 - September 2015</template>
      <template #what>Certifieringskurs inom arkitektur</template>
    </Education>
    <Education>
      <template #header>Certified Scrum Master - Scrum Alliance</template>
      <template #where>Oslo</template>
      <template #when>Januari 2011 - Januari 2011</template>
      <template #what>Certifieringskurs för Scrum Master</template>
    </Education>
    <Education>
      <template #header>VB-Script - QBranch</template>
      <template #where>Stockholm</template>
      <template #when>Oktober 2002 - Oktober 2002</template>
      <template #what>Kurs i VB-script</template>
    </Education>
    <Education>
      <template #header>MSI-paketering - QBranch</template>
      <template #where>Stockholm</template>
      <template #when>Septeber 2002 - September 2002</template>
      <template #what>Kurs i MSI-paketering</template>
    </Education>
    <Education>
      <template #header>SQL Server Administration - Jönsson & Lepp</template>
      <template #where>Stockholm</template>
      <template #when>Oktober 200 - Oktober 200</template>
      <template #what>Kurs i SQL administration</template>
    </Education>
  </CvSections>
  <CvSections>
    <template #icon>
      <CertificationIcon />
    </template>
    <template #heading>Certifieringar</template>
    <CertificationComponent>
      <template #header>Certified IT Architect</template>
      <template #where>IASA Global</template>
      <template #when>2015</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Certified Scrum Master</template>
      <template #where>Scrum Alliance</template>
      <template #when>2011</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Pro: Designing and Developing Web Applications Using Microsoft .NET Framework 4.0</template>
      <template #where>Microsoft</template>
      <template #when>2011</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>TS: Web Applications Development with Microsoft .NET Framework 4</template>
      <template #where>Microsoft</template>
      <template #when>2011</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Analyzing Requirements and Defining Microsoft .NET Solution Architectures</template>
      <template #where>Microsoft</template>
      <template #when>20009</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Designing and Implementing Databases with Microsoft® SQL Server™ 2000 Enterprise
        Edition</template>
      <template #where>Microsoft</template>
      <template #when>2002</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Installing, Configuring, and Administering Microsoft® SQL Server™ 2000 Enterprise
        Edition</template>
      <template #where>Microsoft</template>
      <template #when>2002</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Analyzing Requirements and Defining Solution Architectures</template>
      <template #where>Microsoft</template>
      <template #when>2000</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Designing and Implementing Databases with Microsoft® SQL Server 7.0</template>
      <template #where>Microsoft</template>
      <template #when>2000</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Designing and Implementing Desktop Applications with Microsoft® Visual Basic 6.0</template>
      <template #where>Microsoft</template>
      <template #when>2000</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Designing and Implementing Distributed Applications with Microsoft® Visual Basic 6.0</template>
      <template #where>Microsoft</template>
      <template #when>2000</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Certified Internet Webmaster, Server Administration</template>
      <template #where>ICII</template>
      <template #when>1999</template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Certified Internet Webmaster, Foundations</template>
      <template #where>ICII</template>
      <template #when>1999</template>
    </CertificationComponent>
  </CvSections>
  <CvSections>
    <template #icon>
      <GeneralIcon />
    </template>
    <template #heading>Övrigt</template>
    <CertificationComponent>
      <template #header>Revisor - Bergamasco i Sverige</template>
      <template #where>Jag är revisor för svenska klubben för hundrasen Bergamasco<br>
        <a href="https://www.bergamasco.se" target="_blank">Bergamasco i Sverige</a>
      </template>
    </CertificationComponent>
    <CertificationComponent>
      <template #header>Mensa</template>
      <template #where>Jag är medlem i Mensa Sverige</template>
    </CertificationComponent>
  </CvSections>
  <CvSections>
    <template #icon>
      <ContactIcon />
    </template>
    <template #heading>Kontakt</template>
    Kontaktuppgifter<br>
    Andreas Olausson<br>
    Wahlbecksgatan 6<br>
    582 13 Linköping<br><br>
    Tel: +46(0)720 50 58 00<br>
    <a href="mail:andreas.olausson@ao-tech.se">andreas.olausson@ao-tech.se</a><br>
    <a href="https://www.linkedin.com/in/andreas-olausson/" target="_blank">LinkedIn</a>

  </CvSections>
</template>
