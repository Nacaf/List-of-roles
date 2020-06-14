# List-of-roles
You are given a list of roles as an array and a play script as a string.
Each line of the play script is given as follows: Role: text
The text can contain any characters.
Write a program that will group the lines by roles, number them and return the result in the form of ready-made text (see example). Each group is displayed as follows:
Role:
i) text
j) text2
...
== line feed ==
i and j are line numbers in the script. Indexing lines starts with one, the groups should be displayed in accordance with the order of roles. Line breaks between groups are required, line breaks at the end of the text are not taken into account.
Sample Input:
roles:
["Gorodnichny", "Ammos Fedorovich",
                "Artemy Filippovich", "Luka Lukich"]
textLines:
"City man: I invited you, gentlemen, in order to inform you of the unpleasant news: the inspector is coming to us.
                Ammos Fedorovich: As an auditor?
                Artemy Filippovich: As an auditor?
                Gorodnichy: Inspector from St. Petersburg, incognito. And with a secret order.
                Ammos Fedorovich: Here are those on!
                Artemy Filippovich: There was no care, so give it!
                Luka Lukic: Good heavens! also with a secret order! "
Sample Output:
Mayor:
1) I invited you, gentlemen, in order to tell you unpleasant news: the inspector is coming to us.
4) Examiner from St. Petersburg, incognito. And with a secret order.
 Ammos Fedorovich:
2) How is the auditor?
5) Here are those on!
Artemy Filippovich:
3) How is the auditor?
6) There was no care, so give it!
Luka Lukic:
 7) Lord God! also with a secret order!
