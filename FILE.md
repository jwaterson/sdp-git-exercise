git init<br>
echo ***This is where work is done*** > commitMe.txt<br>
git add .<br>
git commit -m "Commit 0"<br>
git branch bug-fix<br>
echo First bit of work executed in master branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 1"<br>
echo Second bit of work executed in master branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 2"<br>
git checkout bug-fix<br>
echo Third bit of work executed in bug-fix branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 3"<br>
echo Fourth bit of work executed in bug-fix branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 4"<br>
git branch bug-fix-experimental<br>
git merge master<br>
more commitMe.txt<br>
(resolved conflict by manually editing commitMe.txt in editor)<br>
echo Fifth bit of work executed in bug-fix branch >> commitMe.txt<br>
git add commitMe.txt<br>
git commit -m "Commit 5"<br>
echo Sixth bit of work executed in bug-fix branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 6"<br>
git checkout bug-fix-experimental<br>
echo Seventh bit of work executed in bug-fix-experimental branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 7"<br>
echo Eigth bit of work executed in bug-fix-experimental branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 8"<br>
echo Ninth bit of work executed in bug-fix-experimental branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 9"<br>
git checkout master<br>
echo Tenth bit of work executed in master branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 10"<br>
git checkout bug-fix<br>
git merge bug-fix-experimental<br>
(resolved conflict by manually editing commitMe.txt in editor)<br>
echo Eleventh bit of work executed in bug-fix branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 11"<br>
echo Twelfth bit of work executed in bug-fix branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 12"<br>
git checkout master<br>
git merge bug-fix<br>
(resolved conflict by manually editing commitMe.txt in editor)<br>
echo Thirteenth bit of work executed in master branch >> commitMe.txt<br>
git add .<br>
git commit -m "Commit 13"<br>
git add SimpleCommitGraph.png UnabridgedCommitGraph.png FILE.md<br>
