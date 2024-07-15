
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Common Integrated Services</title>
  <style>
    /* Reset default margin and padding */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    
     body {
      font-family: Arial, sans-serif;
      background-color: #f0f0f0;
      color: #333;
      line-height: 1.6;
      padding: 2rem;
    }
    
    header {
      text-align: center;
      margin-bottom: 2rem;
    }
    
    header h1 {
      font-size: 2.5rem;
      color: #004d40;
    }
    
    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1rem;
    }
    
    .service {
      background-color: #fff;
      padding: 2rem;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease-in-out;
      text-align: center;
    }
    
    .service:hover {
      transform: translateY(-5px);
    }
    
    .service h2 {
      font-size: 1.5rem;
      margin-bottom: 1rem;
      color: #004d40;
    }
    
    .service p {
      font-size: 1.1rem;
    }
    
    .service a {
      text-decoration: none;
      color: #333;
      display: block;
      margin-top: 1rem;
      transition: color 0.3s ease-in-out;
    }
    
    .service a:hover {
      color: #004d40;
    }
    
    /* Specific styles for detailed sections */
    .education-section, .healthcare-section, .transport-section, .government-section, .school-directory, .hospital-directory {
      display: none;
    }

    .schools, .hospitals, .routes, .public-transport, .service-centers, .vehicle-renting, .government-services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1rem;
    }
    
    .school, .hospital, .route, .transport, .service-center, .vehicle, .government {
      background-color: #fff;
      padding: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }
    
    .school h2, .hospital h2, .route h2, .transport h2, .service-center h2, .vehicle h2, .government h2 {
      font-size: 1.5rem;
      margin-bottom: 0.5rem;
      color: #004d40;
    }
    
    .school p, .hospital p, .route p, .transport p, .service-center p, .vehicle p, .government p {
      font-size: 1.1rem;
      margin-bottom: 1rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to Common Integrated Services</h1>
    <p>Explore various services for education, healthcare, transport, financial, and government needs.</p>
  </header>
  
  <main id="main-content">
    <section class="services" id="services-section">
      <div class="service education">
        <h2>Education</h2>
        <p>Explore educational resources and services.</p>
        <a href="#" onclick="showEducationServices()">Explore more</a>
      </div>
      <div class="service healthcare">
        <h2>Healthcare</h2>
        <p>Access healthcare services and information.</p>
        <a href="#" onclick="showHealthcareServices()">Explore more</a>
      </div>
      <div class="service transport">
        <h2>Transport</h2>
        <p>Plan your travel and commute easily.</p>
        <a href="#" onclick="showTransportServices()">Explore more</a>
      </div>
      <div class="service financial">
        <h2>Financial</h2>
        <p>Manage your finances and investments.</p>
      </div>
      <div class="service government">
        <h2>Government Services</h2>
        <p>Access government information and services.</p>
        <a href="#" onclick="showGovernmentServices()">Explore more</a>
      </div>
    </section>

    <section class="education-section" id="education-section">
      <h2>Education Services</h2>
      <div class="services">
        <div class="service">
          <h2>School Directory</h2>
          <a href="#" onclick="showSchoolDirectory()">View Directory</a>
        </div>
        <div class="service">
          <h2>Student Profiles</h2>
          <p>View detailed profiles of students.</p>
        </div>
        <div class="service">
          <h2>Online Courses</h2>
          <p>Access a variety of online courses.</p>
        </div>
        <div class="service">
          <h2>Scholarships</h2>
          <p>Find scholarships for your studies.</p>
        </div>
        <div class="service">
          <h2>Internships</h2>
          <p>Explore internship opportunities.</p>
        </div>
        <a href="#" onclick="showMainServices()">Back to Main Services</a>
      </div>

      <section class="schools" id="school-directory" style="display:none;">
        <h2>School Directory</h2>
        <div class="school">
          <h2>School A</h2>
          <p><strong>Location:</strong> City A</p>
          <p><strong>Grade Levels:</strong> K-12</p>
          <p><strong>Contact:</strong> info@schoola.com</p>
        </div>
        <div class="school">
          <h2>School B</h2>
          <p><strong>Location:</strong> City B</p>
          <p><strong>Grade Levels:</strong> K-8</p>
          <p><strong>Contact:</strong> info@schoolb.com</p>
        </div>
        <div class="school">
          <h2>School C</h2>
          <p><strong>Location:</strong> City C</p>
          <p><strong>Grade Levels:</strong> 9-12</p>
          <p><strong>Contact:</strong> info@schoolc.com</p>
        </div>
        <a href="#" onclick="hideSchoolDirectory()">Back to Education Services</a>
      </section>
    </section>

    <section class="healthcare-section" id="healthcare-section">
      <h2>Healthcare Services</h2>
      <div class="services">
        <div class="service">
          <h2>Hospital Directory</h2>
          <a href="#" onclick="showHospitalDirectory()">View Directory</a>
        </div>
        <div class="service">
          <h2>Patient Profiles</h2>
          <p>View detailed profiles of patients.</p>
        </div>
        <div class="service">
          <h2>Reports</h2>
          <p>Access medical reports and records.</p>
        </div>
        <div class="service">
          <h2>Emergency Services</h2>
          <p>Get emergency medical assistance.</p>
        </div>
        <div class="service">
          <h2>Appointments</h2>
          <p>Schedule appointments with doctors.</p>
        </div>
        <a href="#" onclick="showMainServices()">Back to Main Services</a>
      </div>

      <section class="hospitals" id="hospital-directory" style="display:none;">
        <h2>Hospital Directory</h2>
        <div class="hospital">
          <h2>Hospital A</h2>
          <p><strong>Location:</strong> City A</p>
          <p><strong>Contact:</strong> info@hospitala.com</p>
        </div>
        <div class="hospital">
          <h2>Hospital B</h2>
          <p><strong>Location:</strong> City B</p>
          <p><strong>Contact:</strong> info@hospitalb.com</p>
        </div>
        <div class="hospital">
          <h2>Hospital C</h2>
          <p><strong>Location:</strong> City C</p>
          <p><strong>Contact:</strong> info@hospitalc.com</p>
        </div>
        <a href="#" onclick="hideHospitalDirectory()">Back to Healthcare Services</a>
      </section>
    </section>

    <section class="transport-section" id="transport-section">
      <h2>Transport Services</h2>
      <div class="services">
        <div class="service">
          <h2>Routes and Navigation</h2>
          <p>Find routes and navigate easily.</p>
        </div>
        <div class="service">
          <h2>Public Transport and Stations</h2>
          <p>Find information on public transport and stations.</p>
        </div>
        <div class="service">
          <h2>Nearby Service Centers</h2>
          <p>Locate nearby vehicle service centers.</p>
        </div>
        <div class="service">
          <h2>Vehicle Renting</h2>
          <p>Rent vehicles for your travel needs.</p>
        </div>
        <a href="#" onclick="showMainServices()">Back to Main Services</a>
      </div>
    </section>

    <section class="government-section" id="government-section">
      <h2>Government Services</h2>
      <div class="services">
        <div class="service">
          <h2>Government Directory</h2>
          <p>Access contact information for government offices.</p>
        </div>
        <div class="service">
          <h2>Citizen Profiles</h2>
          <p>View detailed profiles of citizens.</p>
        </div>
        <div class="service">
          <h2>Public Records</h2>
          <p>Search public records and documents.</p>
        </div>
        <div class="service">
          <h2>Legal Services</h2>
          <p>Find legal assistance and information.</p>
        </div>
        <div class="service">
          <h2>Social Services</h2>
          <p>Access social services and support.</p>
        </div>
        <div class="service">
          <h2>Licenses and Permits</h2>
          <p>Apply for licenses and permits.</p>
        </div>
        <a href="#" onclick="showMainServices()">Back to Main Services</a>
      </div>
    </section>
  </main>

  <script>
    function showEducationServices() {
      document.getElementById('services-section').style.display = 'none';
      document.getElementById('education-section').style.display = 'block';
    }

    function showHealthcareServices() {
      document.getElementById('services-section').style.display = 'none';
      document.getElementById('healthcare-section').style.display = 'block';
    }

    function showTransportServices() {
      document.getElementById('services-section').style.display = 'none';
      document.getElementById('transport-section').style.display = 'block';
    }

    function showGovernmentServices() {
      document.getElementById('services-section').style.display = 'none';
      document.getElementById('government-section').style.display = 'block';
    }

    function showMainServices() {
      document.getElementById('education-section').style.display = 'none';
      document.getElementById('healthcare-section').style.display = 'none';
      document.getElementById('transport-section').style.display = 'none';
      document.getElementById('government-section').style.display = 'none';
      document.getElementById('services-section').style.display = 'block';
    }

    function showSchoolDirectory() {
      document.getElementById('education-section').style.display = 'none';
      document.getElementById('school-directory').style.display = 'block';
    }

    function hideSchoolDirectory() {
      document.getElementById('school-directory').style.display = 'none';
      document.getElementById('education-section').style.display = 'block';
    }

    function showHospitalDirectory() {
      document.getElementById('healthcare-section').style.display = 'none';
      document.getElementById('hospital-directory').style.display = 'block';
    }

    function hideHospitalDirectory() {
      document.getElementById('hospital-directory').style.display = 'none';
      document.getElementById('healthcare-section').style.display = 'block';
    }
  </script>
</body>
</html>
