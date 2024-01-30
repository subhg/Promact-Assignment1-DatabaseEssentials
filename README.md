
![Erdiagram](https://github.com/subhg/Promact-Assignment1-DatabaseEssentials/assets/113555022/fb2fb036-4087-4882-a5bc-ee91a9e237e9)

1. **User Table:**
   - UserID (Primary Key)
   - Name
   - Email
   - PhoneNumber

2. **Tweet Table:**
   - TweetID (Primary Key)
   - UserID (Foreign Key referencing User.UserID)
   - TextualContent
   - Timestamp
   - OriginalTweetID (Foreign Key referencing Tweet.TweetID)

3. **Like Table:**
   - LikeID (Primary Key)
   - UserID (Foreign Key referencing User.UserID)
   - TweetID (Foreign Key referencing Tweet.TweetID)

4. **Retweet Table:**
   - RetweetID (Primary Key)
   - UserID (Foreign Key referencing User.UserID)
   - OriginalTweetID (Foreign Key referencing Tweet.TweetID)
   - RetweetTimestamp

5. **Follow Table:**
   - FollowID (Primary Key)
   - FollowerID (Foreign Key referencing User.UserID)
   - FollowingID (Foreign Key referencing User.UserID)

