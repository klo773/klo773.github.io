<!DOCTYPE html>
<html>
<body>
<iframe src="https://il11liiillli11.github.io/rbcollegeworking/new.html" style="height:1000px;width:2000px" title="Iframe Example"></iframe>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RetroBowl Button</title>
    <script>
        function modifyCredits() {
            if (localStorage.getItem("RetroBowlCollege.0.savedata.ini")) {
                let z = prompt("How many credits do you have right now (please input the correct number)?");
                localStorage.setItem("RetroBowlCollege.0.savedata.ini", localStorage.getItem("RetroBowlCollege.0.savedata.ini").replace(`coach_credit="${z}"`, 'coach_credit="999999999999"'));
                window.location.reload(); // Reload the page
            } else {
                alert("You must open up a new game save first!");
            }
        }
    </script>
</head>
<body>
    <button onclick="modifyCredits()">Modify Credits</button>
</body>
</html>
