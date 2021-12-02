# Dentistimo
[[_TOC_]]

## What?
A software that keeps track of the availaiblity of free time-slots for dentists in Gothenburg, where the client uses a browser-based application to visualize the locations of the dentists and book a specific dentist by clicking on the marker on the map. A confirmation of the booking will be displayed to the client according to the availablity otherwise a rejection will be displayed.

## Why?
In order to automatically get a list of available dentists according to the time window set by the client.

## How?
The visualiser recieves the dentists registry over the MQTT-protocol.

## Project requirements  <br />
[ SRS ](https://git.chalmers.se/courses/dit355/test-teams-formation/team-8/team-8-project/-/blob/main/SRS.pdf) <br />


## Technologies used
*  MQTT with HiveMQ broker
*  MapBox
*  Node.js

## Developers
* Leila Bencheikh
* Maab Mohammedali
* Mila Mehrvarz
* Muntasir Adam
* Ramzi Abu Zahra

## Project Managment  <br />
[ Trello Board ](https://trello.com/dit355h21group8) <br />



## Software Architecture style

### Publish-Subscribe Architecture Style

publish/subscribe is one of the architecture style that we have considered to implement in our project in order to exchange messages between two components in our system. In this architecture style one component subscribes to a message that has been
published by a publisher(another Component). The publish and subscribe will make use of the MQTT Paho
technology which is one of the core requirements of the project.

### Pipe and Filter Architecture Style

We decided to use the Publish-Subscribe architecture style and the Pipe-Filter style. Using
the pipe and filter will allow more components to be added later on during the course when
the requirements add up over time

## Diagrams describing our project:

## Use-Case Diagram
<br>
<a herf="https://git.chalmers.se/courses/dit355/test-teams-formation/team-8/team-8-project/-/blob/useDiagram/assets/Use-Case%20Diagram.png"><img  src="./assets/Use-Case Diagram.png"><br>

## Sequence Diagram
<br>
<a herf="https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Sequence%20diagram%20and%20activity%20diagram#R7V1dc6M4Fv01rpp9sAtJfD4mTvd012aruibTtbtPWxjkmG6MvCB3kv31KwECJIGNbTAZd%2BchCQIE6N57dHR0ETO03L7%2Bnvq7zT9IiOMZNMLXGXqYQQhc02V%2FeMlbUWLasCh4TqOwPKgueIr%2Bh8tCoyzdRyHOpAMpITGNdnJhQJIEB1Qq89OUvMiHrUksX3XnP2Ot4CnwY730n1FIN0WpC526%2FBOOnjfiysD2ij1bXxxcPkm28UPy0ihCH2ZomRJCi%2F%2B2r0sc88YT7VKc97Fjb3VjKU5onxOyT%2BG3O%2FPPzUdM%2F%2BN8BZ%2F%2B%2Fm07n1t2Uc0PP96XT3xPyPcoeebtl%2FBfux2JErrlV2GV8aIHnERZFm1J%2BWD0TbQWe8Yd%2F3e%2FjT%2Bm%2Fpb9e%2F%2ByiSh%2B2vkBL39hTsLKNnQbsy3Ad5eNChyD7xBNifjWiuyTEIePK3HwD5zSiNnmLo6eE1a2jcKQX%2FreLwtivGZn32fscuwRHvOtB4uVrElCS%2BcCiG9HcbwkMUnz%2B0ahhd3Q5GfSlHzHjT0uXCHbFjWUT1q2Pb8d%2FNppDlAZmUUHJltM0zd2SHnCHDqlY5SRgcrNl9rNgGGWhZuGj7mi0C99%2B7mqvDY%2F%2B6f0gBO8AWrO8MWnUW75bkM%2FRmscRwk3A3t6Zp9o5%2BdNwPbdBZQ35P0OpxG7RcwbNS6P%2F1KXHXMSFtzUZ6ek1XYc%2B7ssWuW3w10lxcE%2BzaIf%2BA%2BcFWY2WvyFkl3tHX%2FyjQfEbUv2lN%2FRssIQ47jLYMCcxmlzGc92kM%2BrHcJLAJC9xNW9BLb4iGOP5SOu5iOaczQsl2NHfgvW%2Fcx6UFyBpHRDnknix01nuFLDd0dApzUsyRROW8DqprBHM4WpmYIhMxXQbDzc9w3baaLznKgLfeyugzbj24GLV%2Bthos42laCzWyzdGnXmSKYGuq2vHHZDtXy3J3eaw5TjDiC3X%2BCNFXfI%2B2UMYQzoGQurlzksNBYMOr%2FMIcxhOV4vY5hjAZU%2BnpD6pK%2Bf%2F4p9kmzt9RrbQau1Q8dbGW292AB9EjLkPslrYx9tfZI1FgwKv5ou7npY4vy4s0%2BJu1Zr6MYAcLSh2%2BS8%2FP0Yw4SolzXc0QjC5Gzt%2FRgDurCXMRx3LHrwyxgNetDPGACMZQ1Pa3scPmMhrNXN%2B6EuvU8LHVB00dUxjySXcLjVvmFK30oT%2BHtKZDbAWjB9%2Bxc%2Ff2GJzX%2Fnm4Zb7X94LS9QbL01txrGLgpfI1rU55VbZXU2KLfr2vjGW2NDrUt1HpyEd1y45s2xw0lR8jHizZwfXziREKNh5Ty8HQ9zC9bsZJ8G%2BIB5SrNTP33Gh7wOGO1ul%2BLYp4xUSVdtc6Ly1C882pokx5H8Fbjewna8%2BseSayzus6wENrRvpd65oqIBT4H%2BomG0ipgh%2FLfGYSU4dN5%2FJeIq16kjpqixjp%2Bq7S7gYUKOrgHuCcecvrIb58Zk7tYadY%2F%2BCsdypAghPWCek0Nbp%2BSectrs13xax83eJLicuykrm1WC5lHs8w5i39xYCMXuQrd0JaPOgSNXQNbrDNOZCo1DmFbvqq4AlzoilfDJWhTI%2BImgdRZ%2BjohxU2HX3JNjH6pcvwNjjoIgNJTOuAP1TgUr7YaBdwWwQhpYLeMo%2BM6KCJ9bnEH7v3s%2BJcosbjztV1mQRissla72lPJjbxHRioA%2FBGnIACocDYJxSK1VqWFEkLMm5oRQ4YQ2OgfTVOcYF8M6VMFLncBWMUyBng4MG8wVdPlwjWmwYUVxlPEbJWv%2Bi%2FcZLMriKImCjN8e30U3mBduSJbvvV3aUwTMYd4D5T5kPgwRUmsFCh8fESScSUCiGueJrQIiXIROHud1D0Jd1sGfATihn23yhwM9GNWQ6HR0FClmK6eiYrailUNHYey9qRg8UlEHFRvM63VV9w9M92nSBoIBIWkYJT7FPyEkOgchMadNsiUHwUMTSpV6V0PDaWU0sEAygkFgXiSjSeDqQediEe0kbBwXC42eWOheCIWXTR%2Fpc3kPUbaL8wHl1k%2B%2F4zQTQ7QSVEjKAn9HkrBIFpXRhw3YYj5cW6WSl4pRHDfXvJh2vWMHALR7zVu9HuXZz%2FwvJdX1arg7wviaN7n1dzeKd0elL%2BA5KlkbBPLm0JaqBVcDPTgt6OniFwCDDBQnFcPgpbDTpS0pE08QLgzLdSGyoGdq00sjDyuRjm5CdKIvUVCBhp8%2FeFhB3k8CJvAwmDDyZCmK5DBI4iIZoK4mqyPQasjJ6JPlDQMkJZ3iKqGpDFhd62ROJXEoHYSOwdaAHGo0kJLpu%2BWiBXKN6kepcOSxHoIaSD1tWPMKWOJcK%2BM49BIl%2FEUiaPtbnvWWrLJdIYzn2tg%2B8X%2F4UZyjADRW4mWeW8QtdOTdCWNhGtYwwtfckbHqaqQHvTdxHJ2lVXVBlYxSyIQno9SkwNQ3XQKNI9fPXVmeQmrK%2B0BpDdp1HFvx9RFmCpE%2BFyDNFPoyTQtuVNlCh8V%2BFqAuUHgUGgjy5IHeXCXtI4LeNGJ%2Fzc%2BAqQz1TAueA3sNRgYlpPOcyxPF3o%2FGhfrq%2FWPxOBmeWK%2B%2FAKdnjQ3mvbpoX2tpHLV2ZEd%2B5LD1ElE%2Btxliyihb1lTXclVf53g3iXDHtHswjpKlzO1cL6tLvF34bjjdWTlcx2cUu7JkWWyeDH5XJHUjkTU1twK5ShV9JyVt11EqMhfqRPxAKWLIMtVLjU%2F8TD2fVSSBhD71ZVEuiIX6H8Q5Zv5WQOfnh7%2FdJlqaHVPmDeXfMexBAHKyjDAxrToZQHoyQLoXTm8uzAb%2BgYUBTxfjLp80kOjikHDp9SR%2FF%2BPqZa8B6YmnaZ5KkadO1CBS8K4SaW4SQOARugVtQ0H9QdBEwLqgW9dDk2klNH3ecCANbUzl62gwmyMpWkBJ3bJtuxdLGsxZulUnbapwxQ%2F5yeYKzaO5p4ZnKMLRhRL89V%2B7EYvWvZ%2FXbox8DbJmxhU8a8pwWszoGOgPPLCyHWUw1Htg5anYc%2BmoanDH1Fee%2BbpjVKUpGTVX7PutSIlaVrtvdVDUISxKM4FjkBpLVaauxmqsaUSkakij6NlnJMR34p2WII%2Bcs8Du%2FYyRxBJFU9EqNY%2FddhVWNbIkbumSTiry2OUFRqX0hVuEKuuwfsOzCh1ZeLlQ7Ra1KCs%2BjYhMk6g3B2fHJk0SGGuo5MkdmqNWMdhrwu3XGVUDtnS1Rp5DY%2FG3jtIta8B81JWnPlXJTsYWZxlf2LlcsJifILKmbhJTjko6npKPO9A7w7Kkc7X8AEHlJuI%2BMvMZQsutiI%2FrKlqRZzrDjPNOyhYYHP2myw1QBSXHuTL1sTQkW278JAcn8SYNXw%2BqxDAhH5WSUv4CTJ6SfpO4dXhtSz5sQ1DufYZKbtIW6rkadumrld7FzFZJ8TiqnVtW1GcNLQKbrw6eF3ySFs5nBV9IFuV9Y7UofsNLtIX1Y%2B5Jn5NP2A%2BrJTOrlflNXqW8Mv%2Bx9VBdw8iHbPw4aSE0%2FjNrWQjtzjIM0zjkZKesrK8IQmbLoume0Hqay56h0VbWt%2FScoM%2FrQpUJvudvnOQ0Rn75RHEF1iK0re3lNl4ueep635Y84KJ6%2Bx5balTE%2FbB5OapNRgxNXV1jRlrC2Z2hm0oR%2FxVblavYyt2wqXbDedg1IlVD7UflgBWhlGxn2gcvDn7ooPwMBjRmyrcPQJ8vY4hQ7g7Z6zmgAOuWT2V4botDArSwu72vI6DZZv1RlsK16k%2FboA%2F%2FBw%3D%3D"><img  src="activity diagram-activity.drawio.png"><br>

## Activity Diagram
<br>
<a herf="https://git.chalmers.se/courses/dit355/test-teams-formation/team-8/team-8-project/-/blob/main/assets/activity%20diagram-activity.drawio.png"><img  src="./assets/Use-Case Diagram.png"><br>

## Component Diagram
<br>
<a href="https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Untitled%20Diagram.drawio#R7V1fd5u4Ev80eUwOkkDAY52223Nvctve5u7u3TdssM0GGxfjJO6nX2EQRkLYcgJCwU57EiNsGWZ%2B80ejmeEK3S5efku81fw%2B9oPoChr%2ByxX6eAWhY9km%2BZONbPMRZEIjH5kloZ%2BPVQZ%2BhL%2BCfBDQ0U3oB%2BtiLB9K4zhKwxU7OImXy2CSMmNeksTP7NumceQzAytvFtQGfky8qD76R%2Bin8%2BLGoL0f%2FxKEszn9ZoDd%2FMzCo28u7mQ99%2Fz4uTKEPl2h2ySO0%2FzV4uU2iDLqsXT53HC2vLAkWKYyH%2FjrCXjOeLb699MSONtPX%2F40Hv53Xczy5EWb4oavII7IfKNVdsnptqAD%2FrnJrnO08JJZuLxCH8hZvHohv43Kb%2FKGjD%2FBS3rtReGseN%2BEXGCQlKen8TK9Xu8YnZ2FMPsonZ%2B8mhV%2Fo%2Fzv5xU%2FpseVjYVXITuFt1iRF1H96DZerOJlxlI6zH6Ep864dl3Jmy5Mf6rnAw%2FhIvidTOp7aZwcoofoXvzw6e1EehsA2uSV6J53t0hHIfM1sODFxyiYZufjpyCZRjvVNA2JykCjebogfz6CjFRJvHogTA4yHWMUF1eo6UyHjbKP3MYRYUI2N%2FK9wJlOyPg6TeLHoHIGT5xgPC2vp6q4qBYKEoKVylChyH4L4kWQJlvyluIsxk7%2BkcKsOCbOj5%2F3Oto2C8U7r%2BjnUht7hV2YlXPvVSd5UWjPEzQpFGhSju7EAqyyl5NSxtHo7yBNt9SyOHSgNCmmgOJ1%2Bh1U7dJEBTUSQhEFi7EkiLw0fGLNpIiqxfd9i8NMqdEvu4Ymw0GTnSCeTtcEcjxTyot%2BPZ9QixbvkHpr1G07Me1U8bZ%2BWfKqrmEWLczd2RH%2B93C9IRfyK%2BjUQHYKnJZ5rJOlnE6ncCK0lD4eYwu3YymvsWEzihZZTk3PI6GiR2azUn%2BTqTR1M5XoVKqeh6m06ny6hVcfKkqbHI7aFtO36Yw%2FgvE6TAOxzHMgO0V42xBFy2RF0aTHFRwBRwAktyunFctL4iL2N9lYh2JonUpRxWLIcs9WJYbucSYl8WbpB36B3ThJ5%2FEsXnrRXRyvCoTvuFQwxdukMWu8gqX%2FIYuWkcMlEe185PPOxu2mXD8G6WROD%2BJNMgm%2BBQlZgxPX5sfKm4TLWXEy3UlRw0lpqcq%2F4jhWUiqzjaugYsLAZ%2BJ8dUi1jA7L4vBREC3%2FVPsgofFSVSiZe9H0NkwmUR0rhJfJ9s%2Fs4Maih%2F%2BvHNIoLy59H6pNAI80abzogwPgctbahVJAIIT1tpW3rbI3rDuBiijoy0GFTBOu1hlvn%2BfEnGZSnJ15TrwVCwnqIZerHG%2B9yuPw0%2FAlw9ooCYjZ9sa7mTOeFjdGvsYaXVkfMyRu0ihcEg%2BYhvBrGqcLa4wszho7AmssMCegK2MMBIpee3%2Frx2a8niThuGmN2a%2FLZUPE8NhFdZdBrccFJfS0QperxNzF52LZJNCR2svit804CtdzPUURAJuN2WsgiyfE7BXI4itoeh6yKAjZay%2BLd%2FEsnOgoh66pnRieEA9UIYa6RwN7EkMksWw4vzgERcvRBSgq3tj1AhQAhFkBtzE7R8eRCCRhVQcciTiOGNmQhTrE2D0jRrQnf3YBCQAswLFBYJlVBiSQhGE%2BQ40vLb9YkfyWW7olcNANtPf%2FkFppFmwbDk%2F%2FBy9hms%2BMbVwc51MbwCqOP77Q68gOtpWDEqTF2OvRSFW1Pmg0TS7mptqaSGxqnoE1QTbPhr6tiX2xJs0B2OPy66qRX8fljYli8XXOwXy8wf2QXnAqAkwtoKQaMBL5EcPX9y7UbPFgKk5IUKnu986faVFnr3D%2BoJbOnwnV6AK%2BLkO1LjAVxyjVGI%2FdZ%2Fd42h1tG6CpwBNRBaba5r1qMEkEModvWHDNH%2BzbsJxjPmT3aWuOy7AZlDUBR6TtFRlwBUnkM%2BBO%2FKI9uvIpW9UKtii8oE%2FBUCK8hqGUQw377lq5uW6LpYZHt%2FvvDw%2Fk%2FBeiO%2B%2B%2FkxejzBVL5MnAWZ4BVIzZhsWbAlgz%2Bcig6VxsjkNXVt8eUPSwsnzENrN8dF334PJRtBDll5OVhYfhIHbpYRjgyHpid9TeClU2WGUr2p24NrHBgNtxXuvmmJZL%2BGWYlmNgbALACw3ChNyGAbHtupbNV%2B01%2BEBteSmOxJb6exEXHvTsavmg1uvebTaoc1vwHTsok%2BL9z%2BvQBS1uTxc7igE04L1%2FvQDksAoJAD7RUh4zpnlkqq5Bo3jrv6eYL3ZOMtrtxnxlLSqtZureopqsBrQkC95aA53Efv%2F7i%2Fmqr5RVBxiLAwxSWyrrSCwlhh%2FXJZ4wxwZBYxClgV1HtPOfL7mz%2B5dZ5SPcVBpFuEBoRXAbL8n77rwts8bP529Y0mexCpbp7Pq7sELVxXoxVANHxp5w4kUfihOL0PejJpSxSqsCAdTWSh8Qgt2w6xZEt4Gq1QxUw1dhgDqDgSi%2B3xIMRps1EbT1OoNAXqBzgUKDH1q2z6sGfWhupxIguKIMgpaAcL%2Bj9jMh2QUCewhgdsMVQFrLoQIDX%2FxHvHj8Tzp53H69i0fGz0%2B%2FXoT9aQ%2F6dkfMNU%2B3XrpXXtuAXdwD7Aq0LhYEWEEbTbmElD45YPQ2SiuKZZsG1o7S9cjKt3CV6aFsWmiQ9cSuPe7Z6B3MbeMCW9DNFQJTodqpxzGK2vqSS2XfizNiFLJdnlFmz4xSvPY%2F3yilzUUpMeBmkY9S0kLixqnai1IKMSNa%2Fr%2FCrayX%2FAczAoyLHwkMi%2FMjMR1Q4UdG8a%2F459fJz7%2B%2B%2F%2Fx7bv7LeUo%2FPbf6nIPWExgGmVdxden63A%2FhP8fJwktv58HkpDyWS%2BPnYT0i4RpwBYAOTY5X8owEoRaGx721zho%2FHzQLurZ66b7xs5As77Hhkt6NCK8BF%2FJxYX2N21nbJSGTe%2Bu6dBByukpi902XhGR5jy3YtW5DiBDLyf7lsLce7AcBd5FDhiyCmIH2cqhtC0Jg6CaDEj0HFMqgfTJBz0IGz7Hur5rddQgr1ewu8UpHUagYumw%2BSVku2n5yl%2Fg%2Bz%2Fs5CEfxIsgG7BUvZRi4L7xIZBgMPxkQAXZ7x8UCi9xRLqCYLRKhovNT9tLCa6oRXgtwjhx21DQeFN%2B14pqnQTce1AdjyLyxoWPQH27zWLZNQWsgkwibDd9eWDQxUBt7MeDKo9fbC0GtkJh6iko%2FuCcuKff1LpVC7awlFcGlFidSjZdLoRA54%2Bi2NFDcIHSAjQWPSjh1qrpPLDStGwuUzp1BeVlrPaJK5BUHGd9pA8E3eRvqwMXvuSu2HzLP%2Bhu%2B%2FSAyzvVx7NuCCLqE%2FjeYhWs6tzAfaUso5wcJOs6pca4f7sblgDd5nO20xtecAVRGc0Lvlu0dJOIC02BNN3ZdWu1ZJb0oBwzwOdntEX%2BYkT1EYzGFxoa0JwRtvEQbPbXcI0JMY0dSFZuKgjgQuOZNvSsOzUzsrrGr%2BK6HHig8rEGOw0fWTVQGH0TbEdE9Z0etW2i%2B66hfawbFcbmtf6te%2F6XWkje3jDg9jx%2FmSrcplZ%2BeFqXfdFxh0MWVyecWaVva8T6pXnSiiONH4kh88ZZ%2B1G2ZRkcIaJNZ51edASxux90R1Dwrrs6QaayutjyjVO%2B6ZsL1VJ9hCQIL2qej6l2gASzMJSKpfC62mMsSqUkqM8ONk2mqVhj7KtEQBDS0F0atazTIdXN7Tv3LokTIQKUswlNpeiayKFinay%2BL%2BtZp2K52ciiR56NSDs2TaXoecjjgvjyNgnU8fbdAy9G4Ku3E2nmCjWvzO6RqI%2FGW4qd6vLeMLGrntUEMNGp76ooRI5H9o28kvjXL7Lr9Pd1bzJdLdd5b5BerKs%2BDXE6Aa6MeSzawIJA1PP2vS8mGOpABO6vZYIAGELTUYutS2ZfzoqHAsi9LQR87cLEUoujqcSFWlHMByt2nnjw9PPQsHVWrSXWI4cNFqhHzrrN0Wlsb2FiztQEecHGeLhUbWFVNloXsG9PdV2ywEUbi5XX2MCfxfQ%2Bypk9NwYa8z6EMXPwmvGoLcqn427Gh5vr1bUGGWfPHFw1U7cdB2yEl88KHKsnaE9rvv3ORN210Y%2BKG9g6OZd9YXFpV1ypgkBWAjaBjXJYWHZb2igyUIRHQpkN0txTbN9A2yv9qcWhLhEb1NUWtlRwYiF3M2NRpad8UkcMkzjIz9mwkhJzfx36QveMf"> <img  src="./Component.png"><br>
*Component Diagram*

### **Components** <br />

[ Visualizer ](https://git.chalmers.se/courses/dit355/test-teams-formation/team-8/visualizer) <br />
[ TimeValidator ](https://git.chalmers.se/courses/dit355/test-teams-formation/team-8/dataHandler) <br />
[ FormatChecker ](https://git.chalmers.se/courses/dit355/test-teams-formation/team-8/formatChecker) <br />
[ BookingHandler ](https://git.chalmers.se/courses/dit355/test-teams-formation/team-8/extractData) <br />

## Setup and running

### Dependencies
1. Node.js & Npm (https://nodejs.org/en/download/)
2. Git (https://git-scm.com/downloads)

### Setup
1. Move the file Global_values in the Documentations folder to the parent directory
2. Move the file registry in the Documentations folder to the parent directory
3. The components (dataHanlder, extractData, formatChecker) can all be setup with command (npm i mqtt)
4. The component (Visualizer) can be setup with command  (npm init) then (npm i serve)
5. Go to package.json and add under scripts property, above the test subproperty the following line "dev": "serve .",



### Running

1. Run each component except for the Visualizer using Node.js by typing the following command:  (node index.js)
2. Go to Visualizer and run it by typing (npm run dev)
3. Open the port that will be displayed in the console
4. Choose website.html from the choices in the web browser

