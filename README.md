# dayli-calenderpragma solidity ^0.6.0;

contract DailyCalendar {
    mapping(uint => string) public dailyEvents;

    function addEvent(uint day, string memory eventDescription) public {
        dailyEvents[day] = eventDescription;
    }

    function getEvent(uint day) public view returns (string memory) {
        return dailyEvents[day];
    }
}
