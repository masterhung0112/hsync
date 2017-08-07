# hsync

#Brief
hsync is a small, powerful utility for file or folder synchronization.
hsync can synchronize the content of one or many folders recursively.

hsync can make incremental backups. Only new/modified/largers files would be copied.
hsync provides some preconfigured modes (Mirror, backup) for common synchronization or backup tasks.
hsync also detect file meta data (POSIX file ownerships/group/permissions) and could preserve them to the destination file/directories.
hsync let you define advanded filters based on filename patterns (textual or regular expression based) to include or exclude files/directories as desired.
hsync provides real-time synchronization option which watchs source directory continously and synchronize the changes into the destination directory if a file/directory is changed.

#Feature List
- Synchronization
	Powerful synchronization algorithm
	Bi-directional (Two way) and mono-directional (One way) synchronization mode.
	Predefined synchronization modes for mostly used synchronization
		Mirror A->B (incremental): Mirrors new and modified files from A to B
		Mirror B->A (incremental)
		Synchronize A <-> B (incremental): Mirros new and modified files in directories A and B to each other.
		Backup A -> B (full): Make a full copy of directory A to directory B
		Restore B -> A (full)
	Compare files based on their modification dates, changes in their meta data or file contents (deep content scan)
	Options for handling symbolic links.
	Option to preserve file meta data
	Option for real-time synchronization, to watch automatically a directory and start synchronization
- Logging
	Advanced logging/reporting facilities. Just select a logging/reporting level and define where to write the log
	Option to log on application level 
	Option to log on each directory level
	Option to define the log leven (how much to log)
