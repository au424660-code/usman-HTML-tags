<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Google Sheet Viewer</title>
  <style>
    body{margin:0;font-family:Inter,system-ui,sans-serif;background:#f5f7fa;color:#111827;padding:20px;}
    .container{max-width:900px;margin:auto;}
    iframe{width:100%;height:600px;border:none;border-radius:10px;box-shadow:0 8px 30px rgba(0,0,0,0.08);}
    h1{font-size:22px;margin-bottom:10px;}
    .muted{color:#6b7280;font-size:14px;}
    .actions{margin-top:12px;display:flex;gap:10px;}
    .btn{padding:10px 14px;border-radius:10px;border:0;background:#2563eb;color:#fff;font-weight:600;cursor:pointer;}
    .btn.secondary{background:#f1f5f9;color:#2563eb;}
  </style>
</head>
<body>
  <div class="container">
    <h1>Google Sheet Viewer</h1>
    <p class="muted">Live CSV display from your Google Sheet.</p>

    <iframe 
      src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRuNWgSHLI-NMT36MzcKGghgaPwJJbPCBeL-OhmUZoLTvrmbsC_EXnk2Es6XTR4UFzN1cOGGZUydyNA/pubhtml?widget=true&amp;headers=false"
      title="Google Sheet Preview">
    </iframe>

    <div class="actions">
      <button class="btn" onclick="window.open('https://docs.google.com/spreadsheets/d/e/2PACX-1vRuNWgSHLI-NMT36MzcKGghgaPwJJbPCBeL-OhmUZoLTvrmbsC_EXnk2Es6XTR4UFzN1cOGGZUydyNA/pub?output=csv','_blank')">
        Download CSV
      </button>
      <button class="btn secondary" onclick="navigator.clipboard.writeText('https://docs.google.com/spreadsheets/d/e/2PACX-1vRuNWgSHLI-NMT36MzcKGghgaPwJJbPCBeL-OhmUZoLTvrmbsC_EXnk2Es6XTR4UFzN1cOGGZUydyNA/pub?output=csv')">
        Copy CSV Link
      </button>
    </div>
  </div>
</body>
</html>
