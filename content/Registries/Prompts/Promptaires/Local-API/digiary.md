   The first [[TexHelpers#Mode Setter|mode]] developed for Texioty. Can be entered with the `dear_sys,` command while in default mode, and exited with `/until_next_time`. Upon exiting this mode, digiary will create a text file according to the current date in the `filesOutput/.diary/` directory with any lines written since starting the digiary mode.

| Command               | Exaplained                                                            |
| --------------------- | --------------------------------------------------------------------- |
| [[#dear_sys,]]        | Starts the diary mode, each texity input is a new line for the entry. |
| [[#/until_next_time]] | Saves the entry as a text file and exits diary mode.                  |
| [[#redear]]           | Read the dated entry text files.                                      |

#### dear_sys,
   Starts diary mode, which allows for texity to add new lines of text to the current date entry. Texity won't accept any commands other than '/until_next_time', so you're able to exit diary mode safely.



#### /until_next_time
   Save the lines added since the start of the diary mode session, then exits diary mode. A dated entry can have multiple timed entries, each time diary mode starts, a new entry will begin for the same dated entry as the current date.


#### redear
   Get a list of dated entry files and decide which date to read.