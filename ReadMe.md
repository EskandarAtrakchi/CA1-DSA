# This read me is created to give a definition for each of the methods in this application 


# Song.java

This class represents a song in the music library with title and artist attributes.

### `Song(String title, String artist)`
Constructor method to initialize a new Song object with the given title and artist.

### `getTitle()`
Getter method to retrieve the title of the song.

### `getArtist()`
Getter method to retrieve the artist of the song.

### `equals(Object obj)`
Overrides the equals method to compare the title and artist attributes for equality using Objects.equals().

### `hashCode()`
Overrides the hashCode method to improve performance (Big O notation) when storing Song objects in collections.

### `toString()`
Overrides the toString method to return a string representation of the Song object.

# Node.java

This class represents a node in a linked list used to store songs.

### `Node(Song song)`
Constructor method to initialize a new Node object with the given song.

### `getSong()`
Getter method to retrieve the song stored in the node.

### `getNext()`
Getter method to retrieve the next node in the linked list.

### `setNext(Node next)`
Setter method to set the next node in the linked list.

# LikedSongsImpl.java

This class implements the LikedSongsInterface and manages a playlist of liked songs.

### `addSong()`
Adds a new song to the liked songs playlist. The user to input the title and artist of the song and handles cases where the input is empty or repeat mode is activated.

### `printPlaylist()`
Prints the liked songs playlist. It iterates over the playlist and displays the title and artist of each song.

### `deleteSong()`
Deletes a song from the liked songs playlist. It allows the user to specify the title and artist of the song to delete and handles cases where the song is not found or repeat mode is activated.

### `countSongs()`
Counts the number of songs in the liked songs playlist and displays the count to the user. It handles cases where the playlist is empty or repeat mode is activated.

### `setRepeat()`
Activates the repeat mode, making the liked songs playlist circular. It updates the next reference of the last node to point back to the head node.

### `setNotRepeat()`
Deactivates the repeat mode, making the liked songs playlist linear. It updates the next reference of the last node to null.

### `searchSong(String title, String artist)`
Searches for a song in the liked songs playlist by title or artist. It takes the user's input the title and artist of the song to search for and displays the search results.

# GenrePlaylistImpl.java

This class implements the GenrePlaylistInterface and manages playlists for different genres.

### `addHipHopSong(Song song)`
Adds a Hip-Hop song to the playlist. It adds the song to the Hip-Hop playlist and handles cases where repeat mode is activated.

### `addPianoSong(Song song)`
Adds a Piano song to the playlist. It adds the song to the Piano playlist and handles cases where repeat mode is activated.

### `deleteHipHopSong(Song songToDelete)`
Deletes a Hip-Hop song from the playlist. It allows the user to specify the song to delete and handles cases where the song is not found.

### `deletePianoSong(Song songToDelete)`
Deletes a Piano song from the playlist. It allows the user to specify the song to delete and handles cases where the song is not found.

### `printHipHopPlaylist()`
Prints the Hip-Hop playlist. It iterates over the playlist and displays the title and artist of each song.

### `printPianoPlaylist()`
Prints the Piano playlist. It iterates over the playlist and displays the title and artist of each song.

### `countHiphopSongs()`
Counts the number of songs in the Hip-Hop playlist and displays the count to the user.

### `countPianoSongs()`
Counts the number of songs in the Piano playlist and displays the count to the user.

### `setRepeat(boolean repeat)`
Sets the repeat mode for both playlists. It updates the next reference of the last node to point back to the head node if repeat mode is activated.

### `searchHipHopSong(String title, String artist)`
Searches for a Hip-Hop song in the playlist by title or artist. It takes the user's input the title and artist of the song to search for and displays the search results.

### `searchPianoSong(String title, String artist)`
Searches for a Piano song in the playlist by title or artist. It takes the user's input the title and artist of the song to search for and displays the search results.
