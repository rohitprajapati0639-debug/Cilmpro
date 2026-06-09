<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ClaimPro</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:#f4f7fc;
}

.header{
background:#0d6efd;
color:white;
padding:15px;
font-size:24px;
font-weight:bold;
text-align:center;
}

.container{
padding:15px;
max-width:1200px;
margin:auto;
}

.cards{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
gap:15px;
margin-top:20px;
}

.card{
background:white;
padding:20px;
border-radius:15px;
box-shadow:0 2px 10px rgba(0,0,0,.1);
text-align:center;
}

.card h2{
color:#0d6efd;
margin-bottom:10px;
}

.section{
background:white;
padding:20px;
border-radius:15px;
margin-top:20px;
box-shadow:0 2px 10px rgba(0,0,0,.1);
}

input,select,textarea{
width:100%;
padding:12px;
margin-top:10px;
border:1px solid #ddd;
border-radius:10px;
}

button{
background:#0d6efd;
color:white;
border:none;
padding:12px 20px;
border-radius:10px;
margin-top:15px;
cursor:pointer;
}

button:hover{
background:#0056d2;
}

table{
width:100%;
border-collapse:collapse;
margin-top:15px;
}

table th,table td{
padding:12px;
border-bottom:1px solid #ddd;
text-align:left;
}

.status-pending{
color:orange;
font-weight:bold;
}

.status-approved{
color:green;
font-weight:bold;
}

.status-rejected{
color:red;
font-weight:bold;
}

.profile{
display:flex;
align-items:center;
gap:15px;
}

.avatar{
width:70px;
height:70px;
border-radius:50%;
background:#ddd;
}

@media(max-width:768px){
.profile{
flex-direction:column;
text-align:center;
}
}
</style>
</head>
<body>

<div class="header">
ClaimPro - Smart Claim Management
</div>

<div class="container">

<div class="cards">

<div class="card">
<h2>128</h2>
<p>Total Claims</p>
</div>

<div class="card">
<h2>86</h2>
<p>Approved</p>
</div>

<div class="card">
<h2>34</h2>
<p>Pending</p>
</div>

<div class="card">
<h2>8</h2>
<p>Rejected</p>
</div>

</div>

<div class="section">
<h2>Create New Claim</h2>

<input type="text" placeholder="Order ID">

<input type="text" placeholder="AWB / Tracking Number">

<select>
<option>Select Marketplace</option>
<option>Meesho</option>
<option>Flipkart</option>
<option>Amazon</option>
<option>Other</option>
</select>

<select>
<option>Select Issue Type</option>
<option>Damaged Product</option>
<option>Wrong Product</option>
<option>Missing Item</option>
<option>Return Issue</option>
</select>

<textarea rows="4" placeholder="Issue Description"></textarea>

<input type="file" multiple>

<button>Submit Claim</button>

</div>

<div class="section">
<h2>Claim History</h2>

<table>

<tr>
<th>Claim ID</th>
<th>Order ID</th>
<th>Status</th>
</tr>

<tr>
<td>CLM001</td>
<td>ORD123456</td>
<td class="status-pending">Pending</td>
</tr>

<tr>
<td>CLM002</td>
<td>ORD987654</td>
<td class="status-approved">Approved</td>
</tr>

<tr>
<td>CLM003</td>
<td>ORD741258</td>
<td class="status-rejected">Rejected</td>
</tr>

</table>

</div>

<div class="section">
<h2>Claim Tracking</h2>

<p>✓ Claim Submitted</p>
<p>✓ Under Review</p>
<p>⏳ Decision Pending</p>
<p>⬜ Claim Resolved</p>

<button>Download PDF</button>
<button>Share WhatsApp</button>

</div>

<div class="section">

<h2>Profile</h2>

<div class="profile">

<div class="avatar"></div>

<div>
<h3>Rohit Kumar</h3>
<p>+91 9876543210</p>
</div>

</div>

<button>Edit Profile</button>
<button>Notification Settings</button>
<button>Logout</button>

</div>

</div>

</body>
</html>
