# Open Session In View

Open Session In View takes a different approach. Instead of letting the business layer decide how it’s best to fetch all the associations that are needed by the View layer, it forces the Persistence Context to stay open so that the View layer can trigger the Proxy initialization.