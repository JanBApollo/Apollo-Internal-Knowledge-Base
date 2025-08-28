<p>
  Apollo’s credit system is designed to keep large enrichment jobs running smoothly.
  In some cases, customers may appear to go slightly over their credit limits while
  a large batch is in progress. This is expected and by design.
</p>
<strong>Last updated:</strong> August 29, 2025 - Checked details timeliness and accuracy.
<h2 id="h_01K2HDYQRQXPA65BP8ZHW76ZTX">How it works</h2>
<ul class="check--list">
  <li>
    When a bulk enrichment job starts,
    <strong>60% of the job’s estimated credits</strong> are marked as
    <strong>pending usage</strong>.
  </li>
  <li>
    Because only a portion is held up front, the job can proceed even if the
    <em>final</em> usage would slightly exceed the remaining credits.
  </li>
  <li>
    When processing finishes, usage is reconciled against the customer’s account
    credits based on the <strong>actual</strong> number of records enriched.
  </li>
</ul>
<p class="tip--message">
  This approach prevents hard stops near the limit and provides a smoother experience
  for large, in-flight enrichments.
</p>
<h2 id="h_01K2HDYQRQYPCKSM6121XJKF51">What admins and agents should expect</h2>
<ul class="check--list">
  <li>
    Seeing a customer account temporarily appear over its limit during a large
    enrichment is normal.
  </li>
  <li>
    Once the job completes, Apollo deducts the actual credits used and updates
    balances accordingly.
  </li>
  <li>
    If the account has reached its limit after reconciliation, subsequent enrichment
    requests may be blocked until credits are added or refreshed.
  </li>
</ul>
<h2 id="h_01K2HDYQRQHWKGFJZKJJGV60NA">Example</h2>
<ul class="check--list">
  <li>
    <strong>Credits remaining:</strong> 1,000
  </li>
  <li>
    <strong>Batch size (estimated 1 credit/record):</strong> 1,100 credits
  </li>
  <li>
    <strong>Pending usage on start (60% of 1,100):</strong> 660 credits
  </li>
  <li>
    The job is allowed to start because only 660 credits are held pending, even
    though final usage (1,100) will slightly exceed 1,000.
  </li>
  <li>
    After completion, Apollo reconciles to the actual usage and updates the balance.
  </li>
</ul>
<h2 id="h_01K2HDYQRQ860TENZBPJZDGVJ5">Note</h2>
<ul class="check--list">
  <li>Temporary overage during large enrichments is intentional.</li>
  <li>
    Sixty percent pending usage allows work to continue without unnecessary interruptions.
  </li>
  <li>
    Final credit usage is always reconciled based on actual records processed.
  </li>
</ul>
<p class="warning--message">
  <strong>Warning:</strong> If the customer’s surplus exceeds
  <strong>25% of their credits</strong>, notify engineers in
  <a href="https://apolloio.slack.com/archives/C01BC294YHG" target="_blank" rel="noopener noreferrer">#xfn-team-monetization</a>
  so they can log the incident. The surplus will remain part of the current billing
  cycle.
</p>
<h2 id="h_01K2HE2Y1RH42WNQ54WQPS8PDN">Reference</h2>
<p>
  <a href="https://apolloio.slack.com/archives/C01BC294YHG/p1753980561102609" target="_blank" rel="noopener noreferrer">Slack announcement</a>
</p>