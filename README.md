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
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract RewardRate {
    uint256 public rate = 100; // example rate

    function setRate(uint256 _rate) external {
        rate = _rate;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract CompoundFlag {
    mapping(address => bool) public autoCompound;

    function setCompound(bool enabled) external {
        autoCompound[msg.sender] = enabled;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract CompoundFlag {
    mapping(address => bool) public autoCompound;

    function setCompound(bool enabled) external {
        autoCompound[msg.sender] = enabled;
    }
}
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract NFTBurn {
    mapping(uint256 => bool) public burned;

    function burn(uint256 tokenId) external {
        burned[tokenId] = true;
    }
}
