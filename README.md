# helm-uninstall-action
GitHub custom action to uninstall helm releases

      - name: Uninstall Helm Release
        id: uninstall_helm
        if: always()
        uses: patriotsoftware/helm-uninstall-action@v1
        with:
          namespace: testmarco
          release_name: testmarco-${{ steps.extract_branch.outputs.clean-branch }}     
