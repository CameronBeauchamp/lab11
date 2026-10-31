# Error table

One row per failure. Fill in every column. You need at least eight rows.

| Scenario | Function that detects it | Error value | What the player sees |
|---|---|---|---|
| Fleet file does not exist | `load_fleet` | `Err(DataError::Io(..))` (kind `NotFound`) | _(example: your row goes here)_ |
|'load_fleet' | 'Err (dataError::Io(...))' | 'Error: could not load data/fleet.txt: Is a directory (os error 21)' |  |  |  |  |
|'load_fleet' | 'Err(DataError::NoShips("data/fleet.txt"))
' | 'Error: could not load data/fleet.txt: no valid ships in data/fleet.txt' |  |  |  |  |
|  |  |  |  |
|Board file contains nine rows  |  |  |  |
| Board file contains an invalid character |  |  |  |
| Scores file does not exist |  |  |  |
| Scores path points to a directory and cannot be written |  |  |  |
Kill is entered at the firing point
Scenarios to cover (add more if you find them):

- fleet file missing
- a directory given as the fleet path
- fleet file with only comments
- fleet file where every line is bad
- board file with nine rows
- board file with a bad character
- scores file missing
- scores file that cannot be written
- `K11` typed at the prompt
