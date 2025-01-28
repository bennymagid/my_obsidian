<%*
const dailiesFolder = "Dailies"; // Specify the folder containing your daily notes
const files = app.vault.getAbstractFileByPath(dailiesFolder).children;

if (files && files.length > 0) {
  let datePattern = /^\d{4}-\d{2}-\d{2}$/; // Regex for YYYY-MM-DD format
  let links = files
    .filter(file => file.extension === "md" && datePattern.test(file.name.replace('.md', ''))) // Filter by date format
    .map(file => `- [[${file.name.replace('.md', '')}]]`) // Display file name as link
    .join("\n");

  tR += `## Links to Dailies\n${links}`;
} else {
  tR += "No files found in the Dailies folder with the specified date format.";
}
%>