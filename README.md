# MG6

1. I believe the entire for loop runs before the Update method finishes. Since Update runs from top to bottom, it'll run once everything inside it finishes; in this case, the for loop. Hence, the game will lag if the for loop is massive. The update won't finish and update the game until the big for loop is done.

2. When the user is jumping over a platform but doesn't fully jump over it, the collider turns back on. Making the character shift until it's no longer touching the platform. This happens because our velocity reaches its peak and slows down to 0, which makes the collider to be enabled in our if statement forcing Unity to snap the character out.
