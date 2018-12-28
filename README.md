# Solidity-Contract
Blockchain short simple contract
//this is the version of solidity which is the latest version
pragma solidity ^0.4.0;
//this shows that what the contract is ballot
contract Ballot{
    /*Solidity provides  a way to define new types in struct 
    its types can be used in mapping and array also*/
    struct User{
        string user;
        uint score;
    }
    //mapping consist of key and value types and we can also start with the other variable type in mapping
    // the other one is address which is the type which can be any of type
    //the third thing is that the struct which name is user is based on mapping on a specific adress
    mapping(address => User) users;
    //then i use the finction to get the constructor
    address[]public Useraccount;
    //now we will make a function which set the User struct
    function setUser (address _address,uint _score,string _user)public{
       // now we make a var which is passed by the mapping =address
       var User = users[_address] ;
     User .score=_score;
     User .user=_user;
    
    Useraccount.push(_address) -1;
}
function getUser() public view returns (address[]){
    return Useraccount;
}
function getUser(address ins) view public returns(string,uint);
    returns (user[ins].user,user [ins]score);
    //nction countUser() view public returns (uint) {
       //rturn Useraccount .length;
}
}
}
}
