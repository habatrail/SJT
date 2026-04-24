BatchTracker Pro v2.5 Guide
I built this tool to streamline batch timing and keep the data organized without the headache of manual logs. It uses a hardware-precision clock to ensure we aren’t losing time to system lag or background tasks.

Running the App
The script is designed to run as a .pyw file so it opens as a clean window without a terminal appearing in the background. If you need to move it to a different machine, just make sure Python is installed and the batch_history.csv (if created) stays in the same folder for easy access.

Standard Workflow
The entire process is controlled by the Spacebar. Pressing it once starts the Loading phase. Pressing it again moves you into the Running phase, and a third press starts the Unloading phase. On the final press, the app automatically logs the completed batch to the table and resets the timer for the next one. If you have Auto-Start checked, it will immediately jump back into the Loading phase for the next batch ID.

Handling Pauses and Errors
If things get backed up or you need to step away, hit the P key. This freezes the timer and the state logic entirely. The app won't let you accidentally hit the Spacebar to advance the stage while it’s paused, which prevents ghost logs. If a batch is ruined or you need to start a specific cycle over, use the Reset Current button to wipe the active timers without losing your history.

Managing Data
The table at the bottom shows every completed run. To grab data for a report, click the rows you need and hit Ctrl+C. I’ve programmed it to sort the data chronologically in the clipboard, so even if you select the newest batches first, they will paste into Excel in the correct 001, 002, 003 order. Use the Export button to save the entire session to a permanent CSV file.
