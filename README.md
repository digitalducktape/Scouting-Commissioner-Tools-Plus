# Scouting Commissioner Tools Plus

## Leader Training Reminders

A single-page tool for unit commissioners. Load a Scouting America **Trained Leaders** status report (CSV) and it will:

- show where the unit stands on training (percent trained, courses missed most, leaders closest to finishing)
- translate course codes such as `SCO_454` or `Y01` into plain course names with direct links to [training.scouting.org](https://training.scouting.org)
- draft a personal reminder email for each leader who still has courses to take, with copy and bulk-copy options
- match its colors to the unit type (Pack, Troop, Crew or Ship)

**Privacy:** the CSV is read in your browser and is never uploaded. The only things saved are your email wording and signature, in your browser's local storage on your own device.

### Use it

Open the GitHub Pages site for this repository, choose your CSV, and start on the Training status tab. "Show example data" loads made-up people if you only want to look around.

### Run it locally

Open `index.html` in a browser. There is no build step and no dependencies other than the Google Fonts stylesheet.

### Notes

- The course catalog (names, minutes, links) is embedded in `index.html` and was collected from the Scouting America training site. If a course code is not in it, the tool lists the code and links to the course page of the same code.
- Classroom courses are treated as complete once the online courses are done, so the emails point leaders to the online curriculum.
