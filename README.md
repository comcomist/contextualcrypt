# contextualcrypt - granted only under the Humanitarian agpl (hagpl) License.
Providing broutforce resistance by combing arguments to form a unique hash as a sysmetric key of segemtns of data. Under the  Humanitarian agpl (hagpl)

License: https://hopeisback.com/#hagpl

# The contextual crypts client: 
* The client adds a path of arguments to a user password for generating a unique strong (symmetric) key used in locking and unlocking well specified data cut to its segments, for increasing its "Segment Safety Factor"  (ssf), as each ssf =  keySize/segmentSize configurated by the user, while providing a management of those different keys.


# The contextual crypt server:    
* 1. The server is temporal. On each successful user Login the asymmetrically encrypted for that user server schedule is sent to the user, where the schedule includes the time of the next alarmed notification event and where the pub key of users can be changed by the user after any login.
* 2. Each user's data are contextual encrypted by user (and not on the server), where
  * 2.1. the user's data sits under the  directory renamed Tuid, being the temporal user id,
  * 2.2. the server has, additionally, the managing salted hmap:  h(password)-> h(Tuid) and
  * 2.3. each user Login arguments are
  * 2.3.1. Tuid,
  *  2.3.2. password,
  *  2.3.3. newTuid,
  * 2.3.4. newPassword.
* 3. User Login is successful only after each of the steps is successful:
  *   3.1. server check for successful matching of h(password) with password and of Tuid with h(Tuid),
  *   3.2. renaming Tuid to newTuid and updating the managing hmap arguments to (newTuid,newPassword),
  *   3.2. user optionally reset pubKey,
  *   3.4. user get the server schedule.
 

