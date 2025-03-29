<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Simple Search Engine</title>
  <style>
    /* General body styling for a Google-like look */
    body {
      font-family: Arial, sans-serif;
      background-color: #fff;
      margin: 0;
      padding: 0;
      display: flex;
      flex-direction: column;
      align-items: center;
      min-height: 100vh;
    }
    /* Header styling */
    .header {
      margin-top: 50px;
      text-align: center;
    }
    .header h1 {
      font-size: 48px;
      margin: 0;
      color: #4285F4;
    }
    .header img {
      vertical-align: middle;
      height: 50px;
      margin-right: 10px;
    }
    /* Search container styling */
    .search-container {
      margin-top: 30px;
      width: 100%;
      max-width: 600px;
      display: flex;
      justify-content: center;
    }
    .search-container input[type="text"] {
      width: 100%;
      padding: 15px 20px;
      font-size: 18px;
      border: 1px solid #ddd;
      border-radius: 24px;
      outline: none;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    .search-container button {
      margin-left: 10px;
      padding: 15px 20px;
      font-size: 18px;
      border: none;
      border-radius: 24px;
      background-color: #4285F4;
      color: white;
      cursor: pointer;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    /* Results container styling */
    .results {
      margin-top: 40px;
      width: 100%;
      max-width: 600px;
    }
    .result-item {
      padding: 15px;
      border-bottom: 1px solid #eee;
    }
    .text-content h3 {
      margin: 0;
      font-size: 20px;
      color: #1a0dab;
      display: inline-block;
    }
    .text-content p {
      margin: 5px 0 0 0;
      font-size: 16px;
      color: #545454;
    }
    .text-content a {
      text-decoration: none;
      color: #1a0dab;
    }
    .text-content a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <div class="header">
    <h1>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/55/Magnifying_glass_icon.svg/1024px-Magnifying_glass_icon.svg.png" alt="Search Icon">
      SEARCH!
    </h1>
  </div>
  <div class="search-container">
    <input type="text" id="searchInput" placeholder="Search for posts...">
    <button id="searchBtn">Search</button>
  </div>
  <div class="results" id="resultsContainer"></div>

  <script>
    // Local array of posts with clickable links
    const allPosts = [
      {
        userId: 1,
        id: 1,
        title: "The Weather",
        body: "The current forecast",
        link: "https://weather.com/weather/tenday/l/baf0545678cc4b90153636d09d40167afa513aa95c4c773bca0d444af32a2f389df021e031835b60bee52a471ff45eeb"
      },
      {
        userId: 1,
        id: 2,
        title: "The News",
        body: "See what is going on now",
        link: "https://www.wsj.com/"
      },
      {
        userId: 2,
        id: 3,
        title: "Learn JavaScript",
        body: "Here is a good way to learn JS!",
        link: "https://www.codecademy.com/catalog/language/javascript?g_network=g&g_productchannel=&g_adid=699379052629&g_locinterest=&g_keyword=how%20to%20learn%20javascript&g_acctid=243-039-7011&g_adtype=&g_keywordid=kwd-488325314592&g_ifcreative=&g_campaign=account&g_locphysical=9004006&g_adgroupid=165097893569&g_productid=&g_source={sourceid}&g_merchantid=&g_placement=&g_partition=&g_campaignid=21287608736&g_ifproduct=&utm_id=t_kwd-488325314592:ag_165097893569:cp_21287608736:n_g:d_c&utm_source=google&utm_medium=paid-search&utm_term=how%20to%20learn%20javascript&utm_campaign=US_-_Exact&utm_content=699379052629&g_adtype=search&g_acctid=243-039-7011&gad_source=1&gclid=Cj0KCQjwtJ6_BhDWARIsAGanmKcCV05WmVe_UMULRGEOWUO1_pRlKtfF_eEo4g43cZfnzGOWLkhDyawaAnOGEALw_wcB"
      },
      {
        userId: 2,
        id: 4,
        title: "National Day",
        body: "Check out what national day it is today!",
        link: "https://www.nationaldaycalendar.com/what-day-is-it"
      },
      {
        userId: 3,
        id: 5,
        title: "Easy Baking Recipes",
        body: "Some easy recipes to cook and follow!",
        link: "https://www.delscookingtwist.com/easy-baking-recipes-with-minimal-ingredients/"
      }
    ];

    const searchInput = document.getElementById('searchInput');
    const searchBtn = document.getElementById('searchBtn');
    const resultsContainer = document.getElementById('resultsContainer');

    /**
     * Displays posts in the results container.
     * @param {Array} posts Array of post objects.
     */
    function displayResults(posts) {
      resultsContainer.innerHTML = '';
      if (posts.length === 0) {
        resultsContainer.innerHTML = '<p>No results found.</p>';
        return;
      }
      posts.forEach(post => {
        // If a link is provided, make the title clickable
        let titleHTML = post.title;
        if (post.link) {
          titleHTML = `<a href="${post.link}" target="_blank">${post.title}</a>`;
        }
        const div = document.createElement('div');
        div.className = 'result-item';
        div.innerHTML = `
          <div class="text-content">
            <h3>${titleHTML}</h3>
            <p>${post.body}</p>
          </div>
        `;
        resultsContainer.appendChild(div);
      });
    }

    /**
     * Filters posts based on search query.
     * @param {string} query The search term.
     */
    function filterPosts(query) {
      return allPosts.filter(post =>
        post.title.toLowerCase().includes(query.toLowerCase()) ||
        post.body.toLowerCase().includes(query.toLowerCase())
      );
    }

    // Search button click event
    searchBtn.addEventListener('click', function() {
      const query = searchInput.value.trim();
      const filtered = filterPosts(query);
      displayResults(filtered);
    });

    // Allow the Enter key to trigger search
    searchInput.addEventListener('keypress', function(e) {
      if (e.key === 'Enter') {
        searchBtn.click();
      }
    });

    // Initial display of all posts when page loads
    window.addEventListener('DOMContentLoaded', function() {
      displayResults(allPosts);
    });
  </script>
</body>
</html>
