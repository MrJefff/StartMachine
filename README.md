**StartMachine** automatically starts all configured machines when the server starts, and allows players with permission to start/stop machines with a command.

## Permissions
- `startmachine.control` -- allows player to stop/start all machines

## Command
- **machines** or **startmachines** -- Turns all machines on/off based on current state

## Configuration
You can configure the settings in the `StartMachine.json` file under the `oxide/config` directory.
```json
{
  "Campfire control (true/false)": true,
  "Drill control (true/false)": true,
  "Fridge control (true/false)": true
}
```

## Localization
The default messages are in the `StartMachine.json` file under the `oxide/lang/en` directory. To add support for another language, create a new language folder (ex. de for German) if not already created, copy the default language file to the new folder, and then customize the messages.
```json
{
  "CommandAlias": "machines",
  "MachinesStarted": "{0} {1} machines have been started",
  "MachinesStopped": "{0} {1} machines have been stopped",
  "NotAllowed": "You are not allowed to use the 'machines' command"
}
```
