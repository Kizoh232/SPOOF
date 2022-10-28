# ------------------------------------------------------------------------------
# Imports
import os
from twilio.rest import Client
# ------------------------------------------------------------------------------
# Configurations
account_sid = "AC41a26e14d0e6e288237d271d3acc5873"
auth_token = "c6b7215f739111856fc03a8e5e7af84b"

# ------------------------------------------------------------------------------
# Setting the client with the configurations
client = Client(account_sid, auth_token)

# ------------------------------------------------------------------------------
# Creating the message
client.messages.create(
    to="+33756987996",
    from_="DAD",
    body="This is a message send from Python"
)
# ------------------------------------------------------------------------------
