pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
    
				// Make the output directory.
				sh "mkdir -p output"

				// Write an useful file, which is needed to be archived.
				writeFile file: "output/usefulfile.txt", text: "This file is useful, need to archive it."

				// Write an useless file, which is not needed to be archived.
				writeFile file: "output/uselessfile.md", text: "This file is useless, no need to archive it."

				
				// Archive the build output artifacts.
				archiveArtifacts artifacts: 'output/*.txt', excludes: 'output/*.md'
            }
        }
        stage('Test') { 
            steps {
    
				// Make the output directory.
				sh "mkdir -p output"

				// Write an useful file, which is needed to be archived.
				writeFile file: "output/usefulfile.txt", text: "This file is useful, need to archive it."

				// Write an useless file, which is not needed to be archived.
				writeFile file: "output/uselessfile.md", text: "This file is useless, no need to archive it."
				
				// Archive the build output artifacts.
				archiveArtifacts artifacts: 'output/*.txt', excludes: 'output/*.md'
            }
        }
        stage('Deploy') { 
            steps {
    
				// Make the output directory.
				sh "mkdir -p output"

				// Write an useful file, which is needed to be archived.
				writeFile file: "output/usefulfile.txt", text: "This file is useful, need to archive it."

				// Write an useless file, which is not needed to be archived.
				writeFile file: "output/uselessfile.md", text: "This file is useless, no need to archive it."

				
				// Archive the build output artifacts.
				archiveArtifacts artifacts: 'output/*.txt', excludes: 'output/*.md' 
            }
        }
    }
}
