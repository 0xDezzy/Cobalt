# Cobalt

## Description
Cobalt is a bot written in sleep for Cobalt Strike and is intended to be ran with agscript as a bot user. It is based off of [001SPARTAN's bot](https://github.com/001SPARTaN/aggressor_scripts) but uses discord instead of slack. It breaks out the commands in a modular structure so that new commands, modules, and functions can be added easily. This wouldn't exist without his work.

## What it does

### Commands
| Command                 | What it does                                               |
|-------------------------|------------------------------------------------------------|
|`!beacons`               | Lists all the beacons on the teamserver.                   |
|`!elevate-all`           | Attempts to evelate all beacons.                           |
|`!get-downloadstring`    | Returns the Download string for a listener.                |
|`!create-downloadstring` | Creates a Download string for a listener.                  |
|`!getVersions`           | Gets the windows version and creates a note on the beacon. |
|`!listeners`             | Prints all the listeners.                                  |
|`!mimikatz`              | Executes mimikatz on a specified beacon.                   |
|`!add-autodump`          | Adds the beacon to the autodump module.                    |
|`!remove-autodump`       | Removes the beacon form the autodump module.               |
|`!notify`                | Turns Discord notifications on or off.                     |
|`!psexec`                | Executes psexec on the specified beacon for a target.      |
|`!screenshot`            | Takes a screenshot of all beacons.                         |

#### !beacons
Args: `none`

Outputs a list of beacon ids.

#### !elevate-all
Args: `<listener>`

Attempts to elevate all beacons using a specified listener.

#### !get-downloadstring
Args: `none`

Returns a list of download strings.

#### !create-downloadstring
Args: `<listener>`

Creates a download string for a specified listener.

#### !getVersions
Args: `none`

Gets the windows version and creates a note on the beacon.

#### !listeners
Args: `none`

Outputs a list of listeners on the teamserver.

#### !mimikatz
Args: `<beacon id(s)>`

Executes mimikatz on specified beacons. 

#### !add-autodump
Args: `<beacon id(s)>`

Adds the specified beacons to the autodump list.

#### !remove-autodump
Args: `<beacon id(s)>`

Removes the specified beacons from the autodump list.

#### !notify
Args: `none`

Enables or disables Discord notifications.

#### !psexec
Args: `<beacon id> <target> <listener>`

Executes PSExec against a target from a specified beacon using the specified listener.

#### !screenshot
Args: `none`

Takes a screenshot of all beacons

## Usage
Run the following command:

```bash
./agscript <TeamServer IP> <TeamServer Port> <Nickname> <TeamServer Pass> <location of bot>/bot.cna 
```