---
{"dg-publish":true,"permalink":"/notes/dataview-query-for-similar-title/","created":"2024-01-03T10:57:23.088+09:00","updated":"2024-01-03T11:13:35.663+09:00"}
---

# Dataview query for similar title

While creating [[Notes/Tomorrow, and Tomorrow, and Tomorrow first impressions\|Tomorrow, and Tomorrow, and Tomorrow first impressions]] I wanted to create a dataview query to list the notes with similar titles. For example, as I write about "Tomorrow, and Tomorrow, and Tomorrow" I want to automatically show the notes that it is related to without using tags. Here is the query that I [Can I use dataview to display all files that have a certain word in the title? : r/ObsidianMD](https://www.reddit.com/r/ObsidianMD/comments/oi2l4n/can_i_use_dataview_to_display_all_files_that_have/).

> [!tip] I have created a template for this as well.

```

dataview  
List 
WHERE contains(file.name,"Paste your title here")
AND dg-publish = true AND file.name != this.name

```

> [!warning] To help with formatting, I had to remove the ``` from the query. Please add it back before using the query.
