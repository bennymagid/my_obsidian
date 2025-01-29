<%*
const dailiesFolder = "Templates"; // Specify the folder containing your daily notes
const files = app.vault.getAbstractFileByPath(dailiesFolder).children;

if (files && files.length > 0) {
  let links = files
    .filter(file => file.extension === "md" )
    .map(file => `- [[${file.name.replace('.md', '')}]]`) // Display file name as link
    .join("\n");

  tR += `## Links to Dailies\n${links}`;
} else {
  tR += "No files found in the Dailies folder with the specified date format.";
}
%>

## Links to Dailies
- [[Daily Quote]]
- [[Display Daily Notes]]
- [[Display Template Notes]]

