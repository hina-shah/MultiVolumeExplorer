
SET(KIT_PYTHON_SCRIPTS
  qSlicerMultiVolumeExplorerModuleHelper.py
  qSlicerMultiVolumeExplorerModuleWidget.py
  qSlicerMultiVolumeExplorerCharts.py
  )

SET(KIT_PYTHON_RESOURCES
  )

#-----------------------------------------------------------------------------
ctkMacroCompilePythonScript(
  TARGET_NAME qSlicerMultiVolumeExplorerModuleWidget
  SCRIPTS "${KIT_PYTHON_SCRIPTS}"
  RESOURCES "${KIT_PYTHON_RESOURCES}"
  DESTINATION_DIR ${CMAKE_BINARY_DIR}/${Slicer_QTLOADABLEMODULES_PYTHON_LIB_DIR}
  INSTALL_DIR ${Slicer_INSTALL_QTLOADABLEMODULES_PYTHON_LIB_DIR}
  NO_INSTALL_SUBDIR
  )
