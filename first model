// SPDX-License-Identifier: MIT
pragma solidity ^0.8;

contract RandomElementArray {
    string[25] public stringArray; // Fixed-size array to store 25 elements from the periodic table

    constructor() {
        // Initialize the array with periodic table elements
        stringArray[0] = "Hydrogen";
        stringArray[1] = "Helium";
        stringArray[2] = "Lithium";
        stringArray[3] = "Beryllium";
        stringArray[4] = "Boron";
        stringArray[5] = "Carbon";
        stringArray[6] = "Nitrogen";
        stringArray[7] = "Oxygen";
        stringArray[8] = "Fluorine";
        stringArray[9] = "Neon";
        stringArray[10] = "Sodium";
        stringArray[11] = "Magnesium";
        stringArray[12] = "Aluminum";
        stringArray[13] = "Silicon";
        stringArray[14] = "Phosphorus";
        stringArray[15] = "Sulfur";
        stringArray[16] = "Chlorine";
        stringArray[17] = "Argon";
        stringArray[18] = "Potassium";
        stringArray[19] = "Calcium";
        stringArray[20] = "Scandium";
        stringArray[21] = "Titanium";
        stringArray[22] = "Vanadium";
        stringArray[23] = "Chromium";
        stringArray[24] = "Manganese";
    }

    // Function to get a random element from the array
    function getRandomElement(uint256 seed) public view returns (string memory) {
        require(seed > 0, "Seed must be greater than 0");
        uint256 randomIndex = uint256(keccak256(abi.encodePacked(block.timestamp, msg.sender, seed))) % 25;
        return stringArray[randomIndex];
    }
}
