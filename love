function checkCompatibility() {
    const name1 = document.getElementById("name1").value.trim();
    const name2 = document.getElementById("name2").value.trim();

    if (name1 === "" || name2 === "") {
        alert("Please enter both names!");
        return;
    }

    // Simple algorithm to calculate compatibility percentage
    let compatibility = 0;
    const combinedNames = name1.toLowerCase() + name2.toLowerCase();

    // Generate a "compatibility score" based on the sum of character codes
    for (let i = 0; i < combinedNames.length; i++) {
        compatibility += combinedNames.charCodeAt(i);
    }

    // Normalize the result to be between 0 and 100
    compatibility = Math.floor((compatibility % 101) * Math.random() * 100);

    // Update the result on the page
    document.getElementById("compatibility-result").innerText = `Compatibility: ${compatibility}%`;
}
