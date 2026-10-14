1. Get data via arxiv api call: (only chrome: space vs %20?)
https://export.arxiv.org/api/query?search_query=au:%22Florian Chudigiewitsch%22&max_results=200

2. Paste query result in string in wordcloud.html

2.5: Remove <title> field from top level, as we only want <title> of papers

3. Open wordcloud.html in Chrome

4. Inspect and copy svg object to file. Header (everything before <g> should be):

<?xml version="1.0" encoding="utf-8"?>
<svg xmlns="http://www.w3.org/2000/svg" width="600" height="400">

<defs>
<style type="text/css">@import url('https://fonts.googleapis.com/css2?family=Crimson+Text');</style>
</defs>

5. Open svg in affinity designer, copy selection, File > New from clipboard, export to png to resources/wc.png, atleast 2000px height.