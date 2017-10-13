node {  
    stage('Build AngularJS') {
        checkout scm
        sh '''echo "Building AngularJs application....."
echo "$WORKSPACE"
ng build
cd dist
echo "Packaging Angular code"
echo "--------------------------------------------------"
jar -cvf DevOpsTools.war *
mv -f DevOpsTools.war $WORKSPACE/DevOpsTools.war
cd $WORKSPACE
ls -ls'''
    }
    
}
