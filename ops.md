https://www.owiki.ms/wiki/Working_with_GitHub

We see that the local git repository we just created is only tracking the remote repository cxe/react-native-windows. To enable us to get updates from Microsoft/react-native-windows, we need to track Microsoft/react-native-windows as well. We do so by running:

git remote add upstream https://github.com/Azure-Samples/contoso-real-estate.git

We can then merge changes from Microsoft/react-native-windows into our local master branch by running the following commands:

git fetch upstream
git checkout master
git merge upstream/master