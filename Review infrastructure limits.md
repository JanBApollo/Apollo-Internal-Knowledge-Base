<p>
  Apollo enforces infrastructure limitations to ensure platform stability, manage
  bandwidth, and maintain consistent performance for all users. These limits are
  designed to prevent system overloads, especially given Apollo’s large customer
  base.
</p>
<p>
  This article outlines current system-wide restrictions that impact filtering,
  selection, exports, imports, and search operations across different plan tiers.
  Representatives can use this guide to understand, explain, and troubleshoot these
  limits efficiently.
</p>
<h2>Platform-wide limits</h2>
<h3>Net New and Total Tab</h3>
  <ul class="check--list">
    <li>Free plan: 25 selection limit</li>
    <li>Paid plans: 10,000 selection limit</li>
    <li>Error: “Number must be less than or equal to 10000”</li>
  </ul>
<p>
  <img src="/guide-media/01JPYZJDNAB6WE08QAJ5MH0ZDY">
</p>
<h3>
  <strong><img src="/guide-media/01JQA5V4D1PEMYCKY4M0DAHF9B"></strong>
</h3>
<h3>Saved Tab</h3>
  <ul class="check--list">
    <li>All plans: 50,000 selection limit</li>
    <li>Error: “Number must be less than or equal to 50000”</li>
  </ul>
<p>
  <img src="/guide-media/01JPYZGJMB5VF39K6FAXVCEMH1">
</p>
<h2>Job title filters</h2>
<h3>Upper Limit on Number of Job Titles</h3>
  <ul class="check--list">
    <li>Max 100 titles included/excluded per search</li>
    <li>200-character limit per job title</li>
    <li>
      Error: "Exceeded limit of including and excluding 100 job titles" or
      "Value too long"
    </li>
  </ul>
<p>
  <img src="/guide-media/01JPZ0JGBF0YN2MS60G482CX9T">
</p>
<h3>Single Job Title Size Limit</h3>
  <ul class="check--list">
    <li>200-character limit of a Single Job Title.</li>
    <li>Error Message: “Value too long.”</li>
  </ul>
<p><img src="/guide-media/01JQ51THGV1TCQ1F3T1SZQ4YSM" alt="image (42).png"></p>
<h3>Non-Alpha Numeric Limitation</h3>
  <ul class="check--list">
    <li>Only a–z, A–Z, 0–9, and double quotes (") are allowed</li>
    <li>Non-alphanumeric characters are restricted</li>
    <li>Error: “Invalid characters used in the filter”</li>
  </ul>
<p></p>
<h2>Keyword filter limit</h2>
  <ul class="check--list">
    <li>Max 150 company keywords</li>
    <li>Error: "q_organization_keyword_tags has X terms..."</li>
  </ul>
<p><img src="/guide-media/01JPYZWGHD0XN8YKS8VM1XF8WJ"></p>
<h2>Account-related filters</h2>
<ul class="check--list">
  <li>
    No more than 10,000 account-related filtering for Net New people. For example,
    Exclude Accounts stage, Exclude Account list, and Exclude account custom
    field filters on Net New people)
  </li>
  <li>
    Error Message: "<strong>You have filtered for Net New people in more than 10000 accounts (Account List/Owner/Stage filters). Our infrastructure cannot accommodate that many accounts on a Net New people search. You are only shown a partial result of your search."</strong>
  </li>
</ul>
<h3>Domain Filter Limit</h3>
<ul class="checl--list">
    <li>No more than 1,000 domains when using the company domain filter at a time.</li>
    <li>Error Message: <strong>“Number of domains provided exceeds the limit of 1000.”</strong></li> 
    <li>Users must split their domain search in several batches of no more than 1,000 at a time.</li>
</ul>
<h2>Export CSV limit</h2>
<ul class="check--list">
  <li>
    Users can export up to 3 million records within a rolling 7-day window. This
    means that at any given time, the system checks how many records have been
    exported over the past 7 days—not on a fixed schedule. If the total exceeds
    3 million, additional exports will be blocked until older exports fall outside
    the 7-day window.
  </li>
  <li>
    Error Message:
    <strong>"Due to infrastructure limitations, you can only export 3 million records per week. We apologize for the inconvenience."</strong><br>
  </li>
  <li>
    Macro Available: <strong>CSV Export 3 Million Records Limit</strong>
  </li>
</ul>
    <h2>Import CSV Limitation</h2>
    <ul class="check--list">
      <li>Refer to the table below:</li>
    </ul>
    <table border="1.5" style="margin-left: 0px; margin-right: auto;">
      <thead>
        <tr>
          <th>
            <strong>ARR</strong>
          </th>
          <th>
            <strong>Limit</strong>
          </th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Free or ARR &lt; $1k</td>
          <td>100k</td>
        </tr>
        <tr>
          <td>ARR &lt; $5k</td>
          <td>500k</td>
        </tr>
        <tr>
          <td>ARR &lt; $20k</td>
          <td>3M</td>
        </tr>
        <tr>
          <td>ARR &lt; $100k</td>
          <td>10M</td>
        </tr>
        <tr>
          <td>ARR = $100k and up</td>
          <td>50M</td>
        </tr>
      </tbody>
    </table>
    <p>
    </p>
    <p>
      <strong><img src="/guide-media/01JPZ0WCZ85EBDEX8Y8V21JYCE" alt="Untitled (48).png"></strong>
    </p>
    <ul class="check--list">
      <li>
        The import limit is calculated based on the number of records imported
        within the previous week and refreshes on a rolling weekly basis.
      </li>
      <li>
        Macros available:
        <strong>100K Import Limit for Free &amp; Low-Tier Plans (≥ $1K), 500k Import Limit (ARR ≥ $5k).</strong>
      </li>
        <h2>Page Limitations</h2>
        <h3>100-page limit</h3>
        <ul class="check--list">
          <li>
            Apollo only allows viewing of the first 100 pages. We recommend
            using more filters to help narrow down their search.
          </li>
          <li>
            Error Message: No error message. Customers will see the maximum
            page they can go to is 100 while having more than 2,500 results
            on their search.
          </li>
        </ul>
        <p>
          <img src="/guide-media/01JPZ12JMYY66FFPD58V34JK0E">
        </p>
        <ul class="check--list">
          <ul class="check--list">
            <li>
              Macro available: <strong>100 page limitation</strong>.
            </li>
          </ul>
        </ul>
        <h3>3-page or 5-page limit (for users on Free plan)</h3>
            <ul class="check--list">
              <li>Apollo only allows viewing of the first 3 or 5 pages.</li>
            </ul>
<h2>Saved Companies</h2>
        <ul class="check--list">
          <li>
            By default, no more than 300,000 saved companies. Since we
            don't charge for saving companies, there’s a restriction
            on how many can be saved.
          </li>
          <li>
            This limit can be increased by Ray in #ray-requests after
            explaining the type of business of the account and why they
            need to have so many saved companies.
          </li>
          <li>
            Error Message:
            <strong>"You have exceeded the maximum # of companies to add. Your limit is 300000."</strong>
          </li>
        </ul>
        <p>
          <img src="https://downloads.intercomcdn.com/i/o/dyws6i9m/1354511628/27cc8857a04e4ddbde549ca5615d/image.png?expires=1742652900&amp;signature=e6c82f4ce4458d917aed31739cfbf47a9a5b9d999c457a20b95acd9ff0af397a&amp;req=dSMiEsx%2FnIddUfMW1HO4zWKjn4elq7k9CBSychOtcxxSAw%3D%3D%0A">
        </p>
        
        <h2>Fields in CRM Enrichment</h2>
        <ul class="check--list">
          <li>200-Field Limit at a time for enrichment</li>
          <li>
            Error Message:
            <strong>"For performance reasons, the number of selections is capped at 200."</strong>
          </li>
        </ul>
        <p>
          <img src="/guide-media/01JPZ1Q3ZVGK2WTBJ575Q479RH" alt="Untitled (49).png">
        </p>
        <h2>Eyeball icon in Gmail</h2>
        <ul class="check--list">
          <li>
            The eyeball icon is no longer showing on Gmail when emails
            are opened.
          </li>
          <li>This was removed due to performance reasons.</li>
        </ul>
        <h2>Blurred out LAST NAMES for Free Plan users</h2>
        <ul class="check--list">
          <li>
            All contacts based in Illinois &amp; Ohio + plus 8 more US
            states (to be added to the list) will have the last names
            blurred out for users who are on Free or Trial Plans.
          </li>
          <li>
            Macro Available:
            <strong>Last name blurred out for free users.</strong>
          </li>
        </ul>
  <h2>Account prospecting limit</h2>
  <p>
    By default, a team can prospect up to <strong>300,000 accounts</strong> directly
    in Apollo. In addition, Apollo ties the prospecting cap to the team’s current
    lead credit balance so that higher-paying customers can prospect more when
    appropriate.
  </p>
  <p>
    <strong>Effective limit formula:</strong><code>prospecting limit = max(300,000 accounts, current lead credits)</code>
  </p>
  <h3</h3>
  <ul class="check--list">
    <li>
      Apollo does not charge credits for prospecting accounts, and customers
      often
      export this data. The cap prevents giving away large volumes of account
      data
      for free.
    </li>
    <li>
      <strong>300k accounts</strong> is sufficient for most teams’ prospecting
      needs.
    </li>
    <li>
      Linking the cap to lead credits allows only high-ARR customers (with
      larger
      credit allocations) to prospect beyond 300k.
    </li>
  </ul>
  <h3</h3>
  <ul class="check--list">
    <li>
      This cap applies to prospecting <strong>inside Apollo</strong>.
    </li>
    <li>
      Customers can still bring <strong>unlimited accounts</strong> via CSV
      uploads
      or CRM syncs; those imports are not constrained by this prospecting cap.
    </li>
  </ul>
  <h3>Examples</h3>
  <ul class="check--list">
    <li>
      Team with <strong>80,000</strong> lead credits → effective limit =
      <strong>300,000</strong> (baseline applies).
    </li>
    <li>
      Team with <strong>500,000</strong> lead credits → effective limit =
      <strong>500,000</strong>.
    </li>
  </ul>
  <h3>Overrides and tiering</h3>
  <ul class="check--list">
    <li>
      Apollo can <strong>manually override</strong> a team’s limit on a case-by-case
      basis, guided by the team’s ARR.
    </li>
    <li>
      The tech team can implement a <strong>tiered system</strong> (similar
      to
      CSV import limits) to standardize higher limits by ARR.
    </li>
  </ul>