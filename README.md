// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract AuctionWinner {
    address public winner;

    function setWinner(address _winner) external {
        winner = _winner;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract RefundStyle {
    bool public refundable;

    function enableRefunds() external {
        refundable = true;
    }
}
